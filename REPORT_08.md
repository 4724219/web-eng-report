# 第8回 Webエンジニアリング
## 学籍番号
4724219
## コンポーネント
import type { Todo } from "../types"; 
import { TodoItem } from "./TodoItem"; 

type TodoListProps = { 
    todos: Todo[]; 
}; 

export function TodoList({ todos }: TodoListProps) { 
    return ( 
      <ul> 
        {todos.map((todo: Todo) => ( 
            <TodoItem key={todo.id} todo={todo} /> 
        ))} 
      </ul>
      ); 
    }
## `TodoItem`のProps型
type TodoItemProps = {
  todo: Todo;
};
## 期限あり・なしの演習 レポート構成画面確認結果
export function TodoItem({ todo }: TodoItemProps) {
  const isOverdue =
    todo.dueDate && new Date(todo.dueDate) < new Date(new Date().toDateString());

  return (
    <li>
      <strong>{todo.title}</strong>
      <span> {todo.completed ? "(完了)" : "(未完了)"}</span>

      {todo.dueDate && (
        <span style={{ color: isOverdue ? "red" : "inherit", marginLeft: "8px" }}>
          期限: {todo.dueDate} {isOverdue && "(期限切れ)"}
        </span>
      )}
    </li>
  );
}
