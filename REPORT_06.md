# 第6回 Webエンジニアリング演習 レポート
## 学籍番号
4724219
## `Todo`型の定義
import type { Todo } from "./types.js"; 

let todos: Todo[] = [ 
    { id: 1, title: "型を定義する", completed: true }, 
    { id: 2, title: "関数を作る", completed: false }, 
    { id: 3, title: "テストを書く", completed: false }, 
]; 

## 未完了件数を返す関数の引数と戻り値の型
export async function countIncompleteTodos(): Promise<number> {
    const currentTodos = await fetchTodos();
    const incompleteTodos = currentTodos.filter((todo) => !todo.completed);
    return incompleteTodos.length;
}
## 未完了件数の実行結果
$ tsx src/index.ts
[
  { id: 1, title: '型を定義する', completed: true },
  { id: 2, title: '関数を作る', completed: false },
  { id: 3, title: 'テストを書く', completed: false }
]
未完了のTODO件数: 2
