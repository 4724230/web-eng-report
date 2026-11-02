# 第5回 Webエンジニアリング演習 レポート

## 学籍番号
4724230

## TODOの配列のコード

```typescript
const todos = [
  { id: 1, title: "TypeScriptを復習する", completed: true },
  { id: 2, title: "配列を学ぶ", completed: false },
  { id: 3, title: "レポートを書く", completed: false },
  { id: 4, title: "課題を提出する", completed: true },
];
```

## TODOを更新した条件

```typescript
for (const todo of todos) {
  if (todo.completed === false) {
    todo.completed = true;
    console.log(`更新後: ${todo.title} [完了]`);
  }
}
```

## 完了件数の更新前後の実行結果

更新前：2件

更新後：4件

実行結果：

```text
完了件数: 更新前 2件 -> 更新後 4件
```
