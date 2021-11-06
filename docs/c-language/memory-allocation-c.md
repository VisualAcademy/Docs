---
description: "동적 메모리 할당"
title: "동적 메모리 할당 (C)"
date: "2021-11-07"
keywords: ["동적 메모리 할당 [C]"]
assetid: 560a8de4-19db-4868-9f18-dbe51b17900f
---

# 동적 메모리 할당 (C)

C 언어에서는 사용자가 직접 동적으로 메모리를 할당하고 사용한 후 할당된 메모리를 해제할 수 있습니다. 이러한 일련의 절차를 **동적 메모리 할당**이라고 합니다. 


## 문법

C 언어에서 동적으로 메모리를 할당할 때에는 **`malloc()`** 함수를 사용합니다. 

동적 메모리 할당 관련 코드 조각은 다음과 같습니다. 

```C
int* num = malloc(sizeof(int));
```

주의할 점은 동적으로 할당된 변수는 반드시 **`free()`** 함수로 메모리 해제를 해주어야 합니다.

```C
free(num);
```

## 예제 

다음 코드는 C 언어에서 **동적 메모리 할당**에 대한 가장 최소한의 코드를 보여줍니다. 

```C
// c_for.c
// memory_allocation.c
// 동적 메모리 할당
#include <stdio.h>
#include <stdlib.h>

int main(void)
{
    //[1] 포인터 변수 선언
    int* num;

    //[2] 메모리 할당
    num = malloc(sizeof(int));

    if (num) // 유효성 검사: NULL이 아니면 num 변수 사용
    {
        //[3] 할당된 공간에 값 대입
        *num = 1234;

        //[4] 포인터 변수의 값 참조
        printf("%d\n", *num);

        //[5] 메모리 해제
        free(num);
    }

    return 0;
}
```

## 실행

```Output
1234
```

## 참고 강좌

C 언어 동적 메모리 할당에 대한 참고 강좌는 다음 경로를 참고하거나 [데브렉](http://www.devlec.com) 사이트의 동영상 강의를 참고하세요. 

- [자바캠퍼스 - C 언어 동적 메모리 할당](https://youtu.be/z7eaCAhqRAY)

- [데브렉](http://www.devlec.com)

