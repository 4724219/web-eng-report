# 第4回 Webエンジニアリング演習 レポート
## 学籍番号
4724219
## `const`と`let`の宣言・再代入に使用したコード
const courseName = "Web Engineering";
let retryCount = 1;

retryCount = 2;

console.log(retryCount);
## VSCodeと`pnpm run check`に表示されたエラー番号・メッセージ
エラー番号: ⁠TS2588⁠ 
エラーメッセージ: ⁠Cannot assign to 'courseName' because it is a constant. 
## 修正後の実行結果と`const`・`let`の違いの説明
const⁠: 定数を宣言するためのキーワード。一度値を代入すると、後から再代入することはできない。
⁠let⁠: 変数を宣言するためのキーワード。宣言後に値を自由に書き換えることができる。