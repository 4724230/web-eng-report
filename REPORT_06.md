# 第6回 Webエンジニアリング演習 レポート
## 学籍番号
4724230
## `Todo`型の定義
export type Todo = {
  id: number;
  title: string;
  completed: boolean;
  dueDate?: string;
};
## 未完了件数を返す関数の引数と戻り値の型
export async function countIncompleteTodos(): Promise<number>
## 未完了件数の実行結果
未完了TODOの件数: 1
