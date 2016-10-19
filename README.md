# 마이크로소프트 봇 프레임워크로 만드는 인공지능 봇
Microsoft Bot fraemwork code for D.Camp - D.Party presentation
이 자료는 d.party 발표를 위해 제작. http://www.dcamp.kr/event/apply/1500  

### 10분 동안 만드는 진짜 Bot
Microsoft Bot Framework를 이용해  
봇을 개발 / 게시 / 등록하고, 실제 메신져 어플리케이션에서 추가해 봇과 채팅하는 어플리케이션을 개발하는 것이 목표

### 전체 진행 절차
Microsoft Bot Framework를 이용해 실제 봇을 개발하는 절차
- Node.js 또는 .NET을 이용해 프로젝트 시작
- .NET 과정일 경우 Bot Framework 템플릿을 이용해 진행
- 봇 에뮬레이터로 테스트(Microsoft Bot Framework Channel Emulator)
![봇 에뮬레이터 이미지](https://docs.botframework.com/en-us/images/connector/connector-getstarted-test-conversation-emulator.png)
- Microsoft Azure - PaaS, App Service의 API App으로 publish 수행
- 봇을 Microsoft Bot Framework에 "등록"
- 등록한 봇을 테스트
- 채널 설정 및 다른 메신저(Facebook Messenger, Skype, Slack, Telegram 등)와 통합
- (시간이 나면) Azure Machine Learning의 Predictive Model로 예측 분석 수행

## 전체 과정 영상
d.party에서 라이브 코딩이 불가할 경우를 대비해 만들어 둔 영상입니다.

## 사용한 코드 정보
https://github.com/CloudBreadPaPa/d-party-bot-framework 리포지토리 하위의 d-party-bot-framework 폴더에 모든 코드 포함  
web.config 파일의 아래 내역 수정 필요
```
<!-- update these with your BotId, Microsoft App Id and your Microsoft App Password-->
<add key="BotId" value="dwkim-bot-d-party" />
<add key="MicrosoftAppId" value="AppID" />
<add key="MicrosoftAppPassword" value="AppPWD" />
```

