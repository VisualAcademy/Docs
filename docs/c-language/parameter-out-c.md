---
description: "포인터로 반환형 매개 변수 전달 방식 함수 만들기"
title: "포인터로 반환형 매개 변수 전달 방식 함수 만들기 (C)"
date: "2021-11-08"
keywords: ["포인터로 반환형 매개 변수 전달 방식 함수 만들기 [C]"]
assetid: 560a8de4-21db-4868-9f18-dbe51b17900f
---

# 포인터로 반환형 매개 변수 전달 방식 함수 만들기 (C)

함수를 호출하기 전에는 굳이 지역 변수를 초기화하지 않고 호출한 함수에서 전달한 값을 받아서 사용해야 하는 경우가 있습니다. 
이런 경우에는 포인터 사용하여 반환형 매개 변수 전달 방식을 사용할 수 있습니다. 


## 예제: parameter_out.c 


```C
//[?] 포인터로 반환형 매개 변수 전달 방식 함수 만들기
// parameter_out.c
#include <stdio.h>

void do_something(int* num)
{
    *num = 1234; // [B] 역참조로 전달된 main 함수의 변수에 저장, 반드시 초기화해야 함
    printf("[1] %d\n", *num); // [1] 1234
}

int main(void)
{
    int num; // [A] 변수를 반드시 초기화할 필요 없음

    do_something(&num); // 반환형 매개 변수 전달 방식: 변수의 주소를 전달 

    printf("[2] %d\n", num); // [2] 1234

    return 0;
}
```

## 실행

```Output
[1] 1234
[2] 1234
```


## 참고


더 많은 온라인 강좌는 [데브렉](http://www.devlec.com) 사이트의 동영상 강의들을 참고하세요. 

- [데브렉](http://www.devlec.com)
- [비주얼아카데미](https://www.visualacademy.com)


