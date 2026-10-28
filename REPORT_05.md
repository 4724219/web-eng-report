# 第5回 Webエンジニアリング演習 レポート
## 学籍番号（学籍番号）
4724219
## TODO配列のコード（コードまたは確認結果）
const todos = [
     { id: 1, title: "型を復習する", completed: true },
     { id: 2, title: "配列を学ぶ", completed: false }, 
     { id: 3, title: "レポートを書く", completed: false },
     { id: 4, title: "勉強する", completed: false },
];
## TODOを更新した 条件(コードまたは確認結果）
const completedTodos = todos.filter((todo) => {
    return todo.completed; 
}).length;
## 完了件数の 更新前後の 実行結果（コードまたは確認結果）
$ tsx src/index.ts
1: 型を復習する [完了]
2: 配列を学ぶ [未完了]
3: レポートを書く [未完了]
4: 勉強する [未完了]
1
[ '型を復習する', '配列を学ぶ', 'レポートを書く', '勉強する' ]
更新後: 配列を学ぶ [完了]
更新後: レポートを書く [完了]
更新後: 勉強する [完了]
完了件数: 更新前 1件 -> 更新後 4件
