# Visual Studio 설치 

프로그래밍할 때 소스 코드를 작성하는데 이러한 소스 코드를 작성할 때는 운영체제에 내장된 기본 편집기 또는 Visual Studio Code 같은 무료 편집기(에디터) 프로그램을 사용할 수 있습니다. 
여러 가지 방식이 있지만 박용준 강사의 강의에서는 무료로 가장 손쉽게 사용할 수 있는 Visual Studio 커뮤니티 버전을 사용합니다. 

```C#
> // Visual Studio: 지구상에서 가장 발달된 소프트웨어 개발을 위한 통합 개발 환경(IDE)
```

## Visual Studio와 Visual Studio Code

Visual Studio는 마이크로소프트의 통합 개발 환경이며 소프트웨어를 개발할 때 사용하는 소프트웨어입니다. 
Visual Studio는 C 언어, C#, ASP.NET, C++, Node.js, Python, JavaScript, TypeScript 등의 주요 프로그래밍 개발 환경을 제공합니다. 

### 크로스 플랫폼 개발 환경

C/C# 등 대부분의 프로그래밍 언어는 크로스 플랫폼을 지원하기에 이 강의의 모든 코드는 Windows, Mac, Linux에서 컴파일할 수 있습니다. Visual Studio는 Windows용이지만 Visual Studio for Mac과 같이 맥용 프로그램도 제공합니다. Linux에서 프로그래밍을 하려면 Visual Studio Code를 주로 사용합니다.

###	편집기(Editor)와 통합 개발 환경(IDE)

간단한 텍스트를 편집하는 도구를 편집기(에디터)라고 부릅니다. 
이러한 에디터를 포함해서 프로그램을 작성할 때 필요한 편집기 및 디버거 등의 모든 기능을 다 제공하는 소프트웨어를 통합 개발 환경(Integrated Development Environment)이라고 하는데 줄여서 IDE라고 부릅니다. 
Visual Studio가 대표적인 IDE입니다.

- 편집기: Visual Studio Code
- IDE: Visual Studio

###	Visual Studio Code
Visual Studio Code는 크로스 플랫폼을 제공하여 윈도, 맥, 리눅스 운영체제에서 모두 사용할 수 있는 전세계에서 가장 많은 개발자들이 사용하는 코드 편집기입니다. Visual Studio Code는 폴더 자체를 하나의 프로젝트로 인식하여 엽니다.



## Visual Studio Community 버전 설치하기

마이크로소프트는 Visual Studio의 무료 버전인 Community 버전을 제공합니다. 
Visual Studio Community 버전의 한국어판은 다음 경로에서 무료로 내려 받아 사용할 수 있습니다. 

- https://www.visualstudio.com/downloads/

###	Visual Studio 다운로드

Visual Studio는 2가지 경로를 통해서 얻을 수 있습니다.

하나는 완성된 정식 버전이고 또 다른 하나는 새롭게 준비되는 기능까지 포함된 미리보기 버전입니다. 

- 정식 버전 다운로드(http://www.visualstudio.com/downloads)
- 미리보기 버전  다운로드(http://www.visualstudio.com/preview)

### 강의 버전

- C 언어 강의는 Visual Studio 2022 버전을 기준으로 제작되었습니다. 하지만, C 언어는 하위 호환성이 잘 되어 있기에 이 강의의 소스는 앞으로 나올 Visual Studio 다음 버전에서도 작성 후 실행이 가능합니다.
- C# 강의는 Visual Studio 2022 버전을 기준으로 제작되었습니다. 하지만, C#은 하위 호환성이 잘 되어 있기에 이 강의의 소스는 앞으로 나올 Visual Studio 다음 버전에서도 작성 후 실행이 가능합니다.


##	[실습] Visual Studio 2022 다운로드 및 설치   

###	소개  

프로그래밍 학습을 위한 개발 도구인 Visual Studio의 최신 버전을 내려받아 설치하는 과정을 진행합니다. 
이 강의의 집필 시점에서는 Visual Studio 2022가 최신 버전이지만, 이후의 버전도 진행사항은 비슷할거라 봅니다. 


#### 참고: Visual Studio 2022 다운로드 및 설치하기 동영상 강좌   

Visual Studio Community 2022를 내려 받고 설치하는 과정을 동영상 강좌로도 마련하였으니 참고하기 바랍니다. 

https://youtu.be/rrG0reVxq3s


#### 따라하기: Visual Studio 2022 다운로드 및 설치   

(1) Visual Studio 다운로드 사이트는 다음 그림과 같습니다. 웹 브라우저를 열고 다음 경로를 주소 창에 입력하여 접속합니다. 

- https://www.visualstudio.com/downloads/ 
 

[그림] Visual Studio 다운로드 사이트 


(2) <Visual Studio 2022 커뮤니티 무료 다운로드> 링크를 클릭하면 설치 파일을 내려 받을 수 있습니다. 
참고로 설치 파일명은 시간이 지남에 따라서 다를 수 있습니다. 
설치 파일을 기본값으로 다운로드를 받습니다. 


(3) 다음 그림과 같이 Visual Studio 설치 파일을 다운로드합니다. 


[그림] Visual Studio 설치 파일 다운로드 


(4) 내려 받은 설치 파일을 더블 클릭하여 실행하면 다음 그림과 같이 Visual Studio Installer를 통해서 설치가 시작됩니다.
 
[그림] Visual Studio Installer 실행


(5) 사용 조건에 동의하기 위해서 <계속> 버튼을 클릭합니다. 
Visual Studio 설치 옵션을 나타내는 워크로드 선택화면에서는 학습하고자하는 프로그래밍 언어에 대한 옵션을 선택하면 됩니다. 
Visual Studio Community 2022에서 추가적으로 필요한 기능을 선택합니다. 

- C 언어는 <C/C++ 데스크톱 개발>을 선택한 후 <설치> 버튼을 눌러 설치를 계속 진행합니다. 
- C#은 <.NET 데스크톱 개발>을 선택한 후 <설치> 버튼을 눌러 설치를 계속 진행합니다. 

용량이 크기 때문에 설치하는 데 시간이 오래 걸립니다.
 
[그림] 워크로드 선택 



(6) 설치가 완료되면 Visual Studio Installer에 다음과 같이 Visual Studio Community 2022 목록이 추가됩니다. 


[그림] Visual Studio Installer에 설치된 버전 리스트 표시 



(7) 설치가 완료되면 시작 버튼을 클릭한 후 설치된 앱에서 Visual Studio 2022을 찾은 후 클릭하여 Visual Studio 2022을 시작합니다. 



(8) 처음 Visual Studio 2022를 실행하면 마이크로소프트 계정으로 로그인해야 합니다. 일단 <나중에 로그인>을 클릭하여 진행합니다.
 
[그림] Visual Studio 실행


Visual Studio에 마이크로소프트 계정으로 로그인하지 않으면 한 달 동안 평가판으로 사용할 수 있습니다. 평가판 사용 기한이 끝나면 라이선스를 업데이트하라는 경고 메시지가 출력됩니다. Visual Studio를 무료로 제한없이 계속 사용하려면 반드시 마이크로소프트 계정으로 로그인합니다.

(9) 마이크로소프트 계정으로 로그인하지 않았다면, 개발 설정에 대한 테마를 선택하는 부분이 나타납니다. 

- C 언어 강의에서는 개발 설정으로 Visual C 언어, 색 테마로 시스템 기본값을 선택하였습니다. 
- C# 강의에서는 개발 설정으로 Visual C#, 색 테마로 시스템 기본값을 선택하였습니다. 
- ASP.NET 강의에서는 개발 설정으로 ASP.NET, 색 테마로 시스템 기본값을 선택하였습니다. 

만약 여기서 개발 설정을 다르게 선택하면 이후 메뉴 구성이 조금 다를 수 있습니다. 

개발 설정 및 테마는 실행 후 <도구 > 설정 가져오기 및 내보내기> 메뉴에서 <모두 다시 설정> 옵션을 선택하면 다시 설정할 수 있습니다. 


[그림] Visual Studio 색 테마 선택


처음 실행하면 테마를 설정할 수 있습니다. 각자 마음에 드는 테마로 설정하면 되며, 이 강의에서는 다음과 같이 설정합니다.
- 개발 설정(V): Visual C 언어
- 색 테마: 파랑

개발 환경 설정 변경은 다음 절차를 사용하여 변경이 가능합니다. 
- <도구 > 설정 가져오기 및 내보내기 > 모두 다시 설정 > 아니요, 다시 설정하여 현재 설정을 덮어씁니다.>에서 변경할 수 있습니다. 
- <도구 > 옵션 > 환경 > 일반 > 색 테마>에서 색 테마를 변경할 수 있습니다. 


(10) Visual Studio 2022 시작 페이지가 실행되었습니다. 오른쪽 하단의 <코드를 사용하지 않고 계속> 메뉴를 클릭하면 메인 화면으로 이동합니다. 


[그림] Visual Studio 시작 화면


(11) 다음 그림은 Visual Studio 2022의 메인 화면입니다. 
 

(12) 참고로, 글꼴 변경은 Visual Studio 메뉴의 <도구 > 옵션 > 환경 > 글꼴 및 색 > 글꼴>에서 글꼴을 변경할 수 있습니다. 

필자는 기본 글꼴을 사용하거나 Consolas 글꼴로 변경을 하였습니다. 

 
[그림] Visual Studio의 텍스트 편집기 글꼴 및 크기 변경 


###	마무리  

여러 C 언어 개발 환경의 첫 번째 방법이자 이 강의에서 사용하는 도구인 Visual Studio의 최신 버전을 설치해 보았습니다. 


## 요약  

Visual Studio를 설치했다면, 프로그래밍 학습을 위한 최고의 도구가 준비된 것입니다. 

다음부터는 실제 코드를 작성하면서 프로그래밍의 기능들을 하나씩 학습해 나가도록 하겠습니다. 

