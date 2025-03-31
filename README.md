[all about oscp](https://www.youtube.com/watch?v=ylrZFMgiFRk)

# OSCP
OSCP 준비
2) Windows Server 2016 & Windows 10

ISO 파일 다운로드 및 설치

 

 

# Windows server 2016

https://www.microsoft.com/ko-kr/evalcenter/download-windows-server-2016

 

- 설치 과정 중 선택 사항

운영 체제 : Windows Server 2016 Standard Evaluation (Desktop Expeirence)

설치 유형 : Custom

 

 

 

# Windows 10

https://www.microsoft.com/en-us/software-download/windows10

 

페이지 접속 후 Downlaod Now 버튼 누르면

 설치 도구 파일이 먼저 받아지면서

해당 도구를 통해 ISO 용으로 변환해야 하는

번거로움이 있으니 이렇게 하지 말고

 

개발자 도구 열어 아래 스텝대로 진행,
사용자 에이전트를 윈도우 이외의 것으로 바꾸면

ISO 파일로 바로 다운로드가 가능하다!

- 설치 과정 중 선택 사항

운영 체제 : Windows 10 Pro

설치 유형 : 사용자 지정 (고급)

정품 인증 : 제품 키가 없음

어떤 설정: 개인용 설정

계정 추가 : 오프라인 추가

로그인 유도 : 제한된 환경

 

 

 

 

3) 서버 환경 및 AD 환경 구축

 

# WIndows Server 2016

- AD 환경 설정


- Domain Controller 설정

- 끝나면 재부팅 됨!

-  재부팅 후 윈도우 서버에서 생성한

AD 도메인 사용자로 로그인 시도(testerA)

정상적으로 도메인 연결에 성공했고

이런 방법으로 다른 서버나 사용자를

하나의 AD 도메인으로 연결해 줄 수 있다.
VPN을 통해 박스에 접근하는 방식이나

시스템 등이 서로 비슷해 별 어려움이나

이질감 없이 PWN Lab 사용이 가능했기

때문.

 

 

 

또한 vulnhub 이상으로 HTB에서

배운 것이 더욱 많았는데 오늘 풀어본

ALPHA 머신에서 그 효과를 톡톡히 보았다.

 

 

 

고로 혹 OSCP를 준비하시는 분이 계시다면

핵더박스를 먼저 경험해 보시고 OSCP

과정으로 넘어가시는 것을 추천드린다.

 

 

 

 

 

 

랩 머신을 사용하는 팁을 남겨본다.

 

 

 

Lab Control Panel에 접속하면

메뉴중에 'MY CLIENTS'와 'PUBLIC SERVERS'가

있고 접속하려는 IP의 머신을 revert, 재기동 시킬 수

있으며 하루에 총 12번(연장 가능) 사용이 가능하다.

 

 

 

MY CLIENTS의 경우는

OffSec에서 개인에게 제공하는

학습용 윈도우 2016 / 10 서버,

그리고 데비안 서버이며

 

 

 

 

사용 하려는 서버를 선택 후

반드시 revert 시켜줘야 사용이 가능하고

접속할때는 터미널에서 'rdesktop'

명령어를 통해 붙으면 된다.

┌──(root💀takudaddy)-[~]
└─# rdesktop 192.168.xxx.xx -g 1024x768    

또는

┌──(root💀takudaddy)-[~]
└─# rdesktop 192.168.xxx.xx -u user -p password -g 1024x768 -x 0x80
 

 

 

PUBLIC SERVERS의 경우는

다른 사람들과 공유해 쓰는 머신이다 보니

먼저 다녀간 사람들이 남긴 불필요한 흔적이

더러 있는 듯하니 접속 전에 reverting을 한 후

사용하도록 하자.

 

 

 

PWN Lab에는

70개 이상의 취약 머신이 존재하며

그중에서 대표로 선발된 11개의 머신이 있는데

오늘 풀어본 ALPHA가 그중 하나였다.

 

 

 

 

 

 

 

제공받은 자료들과 동영상을

조금 훑어본 후 가장 먼저 한 일은

영문 보고서 틀을 만든 것이다.

 

 

 

아무래도 영어로 작성해야 하니

계속 신경이 쓰이던 차에

미리 해 둬야겠다는 생각이 들어

OffSec에서 제공해 주는 샘플 +a

를 참조해 만들었다.
