---
description: "포인터 시작"
title: "포인터 시작 (C)"
date: "2007-01-10"
keywords: ["포인터 시작 [C]"]
assetid: 560a8de4-20db-4868-9f18-dbe51b17900f
---

# 포인터 시작 (C)

2007년 01월 10일 오프라인 강의했던 자료입니다. 


## 예제 


```C
// 포인터시작.c
// pointer-start-c.c 
#include <stdio.h>

int main(void)
{
    int a, b, c; // 값형 변수
    int* p; // 포인터(참조;주소)형 변수

    a = 100;
    b = 200;

    p = &c;

    c = a + b;

    printf("a : %d\n", a);
    printf("b : %d\n", b);
    printf("c : %d\n", c);
    printf("p : %p\n", p); // 번지
    printf("*p : %d\n", *p); // 참조하고 있는 공간의 값 == 역참조 

    return 0;
}
```

## 실행

```Output
 a: 100
 b: 200
 c: 300
 p: 00EFFE80
*p: 300
```

## 참고 강좌

C 언어 포인터 시작에 대한 참고 강좌는 다음 경로를 참고하거나 [데브렉](http://www.devlec.com) 사이트의 동영상 강의들을 참고하세요. 

- [자바캠퍼스 - C 언어 동적 메모리 할당](https://youtu.be/z7eaCAhqRAY)

- [데브렉](http://www.devlec.com)

