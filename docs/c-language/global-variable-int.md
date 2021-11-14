# 전역 변수 만들기 (C)

C 언어에서 전역 변수(Global Variable)는 프로그램의 내부 상태 값을 저장해 놓는 역할을 합니다. 

```C
> // 전역 변수: main() 함수 밖에서 선언된 변수로 모든 함수에서 공유해서 사용 가능한 변수
```

##	지역변수와 전역변수 

C 언어에서 변수를 선언할 때에는 main() 함수와 같은 함수 내에서 선언하거나 함수 밖에서 즉, 함수와 동등한 레벨에서 변수를 선언할 수 있습니다. 함수 내에서 선언된 변수 또는 배열을 지역변수(Local Variable)라고 하며 함수 밖에서 선언된 변수를 전역변수(Global Variable)라고 부릅니다. 전역 변수는 선언 후 초기화하지 않아도 자동으로 초기화됩니다. 예를 들어 int 형 필드는 0으로 초기화됩니다. 


##	지역 변수와 전역 변수 만들기 

지금까지 우리가 사용해 온 변수는 main 함수가 종료되면 자동으로 소멸됩니다. 변수가 살아 있는 영역은 함수의 중괄호 시작과 끝 사이의 영역입니다. 특정 지역의 범위를 가지기에 변수를 일반적으로 지역 변수라고 표현합니다. 

다음과 같이 코드를 작성하고 실행해 보세요. i, j, k의 3개의 지역 변수를 선언 및 초기화하고 3개의 값을 더해서 출력하는 내용입니다. 변수의 값을 더하기(+) 기호를 사용하여 합한 후 출력합니다. 

### 예제: local_variable.c 

```C
// local_variable.c
#include <stdio.h>

int main(void)
{
    int i = 1234;
    int j = 2345;
    int k = 3456;

    printf("%d\n", i + j + k); // 7035

    return 0;
}
``` 
### 실행 
```Output
7035
```

변수는 변수가 선언된 블록(중괄호 열고 닫고({}))안에서만 살아 있습니다. main() 함수에서 선언된 변수는 main() 함수가 종료되면 자동으로 소멸됩니다. 


다음 코드는 C 언어에서 **전역 변수 만들기**에 대한 가장 최소한의 코드를 보여줍니다. 
### 예제: global-variable-int.c 

```C
// global-variable-int.c
// 지역 변수(Local Variable): 함수 안에서 선언된 변수  
// 전역 변수(Global Variable): 함수 밖에서 선언된 변수 
#include <stdio.h>

int global_variable; // 전역 변수 선언(기본값으로 초기화)

int main(void)
{
    int local_variable = 1234; // 지역 변수 선언과 동시에 초기화

    printf("지역 변수: %d\n", local_variable); // 1234
    printf("전역 변수: %d\n", global_variable); // 0

    return 0; 
}
```
### 실행 
```Output
지역 변수: 1234
전역 변수: 0
```


## 참고 강좌

C 언어에 대한 더 많은 강좌들은 다음 사이트를 참고하세요. 

- [데브렉](http://www.devlec.com)

- [자바캠퍼스 - C 언어 강좌](https://www.youtube.com/playlist?list=PLv3VfF96ta72vQdF_gq_YKmeafAIX4970)
