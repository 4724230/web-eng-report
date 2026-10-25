# 第4回 Webエンジニアリング演習 レポート
## 学籍番号
4724230
## `const`と`let`の宣言・再代入に使用したコード
const courseName = "Web Engineering";
let retryCount = 1;

courseName = "Other Course";
retryCount = 2;

console.log(`Course: ${courseName}`);
console.log(`Retry count: ${retryCount}`);
## VSCodeと`pnpm run check`に表示されたエラー番号・メッセージ
error TS2588: Cannot assign to 'courseName' because it is a constant.
## 修正後の実行結果と`const`・`let`の違いの説明
Course: Web Engineering
Retry count: 2

constとletの違い
constは宣言した変数に値を再代入できない。let は値を再代入できる。
