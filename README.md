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
