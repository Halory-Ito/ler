---
title: C++ 中基础 API
draft: true
category: CS
tags:
  - CPP
published: 2025-12-14
---
# 计算类

## 转换类

### 字母大小写转换

在 C++ 中，如果要将一个字母的大小写互换，一般都会利用 ASCII 码的数字进行运算，小写字母 a 对应 65 ，大写字母 A 对应 97 ，两者转换只需要 $\pm 32$ 即可：
```cpp
#include <cstdio>
using namespace std;
int main() {

  char a = 'a';
  char A = 'A';
  printf("%c", a - 32); // A
  printf("%c", A + 32); // a

  return 0;

}
```

