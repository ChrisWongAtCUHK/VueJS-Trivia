---
title: Caveats
---

## 1. 前言

Caveats，就是注意事項。

## 2. 官網
[Reactivity in Depth](https://vuejs.org/v2/guide/reactivity.html#For-Arrays)這樣說：
Vue cannot detect the following changes to an array:

1. When you directly set an item with the index, e.g. <span style="color:#d63200;">vm.items[indexOfItem] = newValue</span>
2. When you modify the length of the array, <span style="color:#d63200;">e.g. vm.items.length = newLength</span>

請看[這裡](https://codesandbox.io/s/intelligent-villani-lye14)。這是個很多人都知道的「特性」。解決方法官方也有。
Solution 1和Solution 2都是官方有的方法，Solution 3是我的方法，缺點是只能做到shallow clone。
