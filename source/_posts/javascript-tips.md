---
title: JavaScript编程技巧
date: 2025-12-21
categories: programming
tags:
  - 编程
  - Js
toc: true
---

# JavaScript编程技巧

本文分享一些实用的JavaScript编程技巧。

## 1. 数组去重

```javascript
const uniqueArray = [...new Set(array)];
```

## 2. 简化条件判断

```javascript
// 传统写法
if (value === 'apple' || value === 'orange' || value === 'banana') {
  // ...
}

// 简化写法
if (['apple', 'orange', 'banana'].includes(value)) {
  // ...
}
```

## 3. 可选链操作符

```javascript
const user = {
  profile: {
    name: 'John'
  }
};

// 传统写法
const userName = user && user.profile && user.profile.name;

// 使用可选链
const userName = user?.profile?.name;
```

## 4. 空值合并操作符

```javascript
const name = null ?? 'Default Name';
```

## 总结

JavaScript提供了许多简洁的语法糖，合理使用可以让代码更加简洁易读。