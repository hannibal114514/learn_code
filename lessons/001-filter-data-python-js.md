# 001 — 保存、筛选、输出：Python vs JavaScript

## Python

```python
scores = [82, 59, 91, 68, 77]
passed = [score for score in scores if score >= 60]
print(passed)
```

## JavaScript

```javascript
const scores = [82, 59, 91, 68, 77];
const passed = scores.filter(score => score >= 60);
console.log(passed);
```

## 必需知识

两段代码做的是同一件事：

1. `scores` 保存一组数字。
2. 从中筛选出 `>= 60` 的数字，保存到 `passed`。
3. 输出 `passed`。

Python 的 `[score for score in scores if ...]` 叫列表推导式；这里先把它读成“从 scores 逐个拿 score，条件满足就留下”。

JavaScript 的 `.filter(...)` 是数组的筛选方法；`score => score >= 60` 是一个很短的函数，意思是“给我一个 score，我判断它是否至少为 60”。

## Reading question

不运行代码：这两段程序最终会输出什么？
