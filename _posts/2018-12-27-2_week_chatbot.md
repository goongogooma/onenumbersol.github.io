---
layout: post
title: SSAFY_2주차_나만의 챗봇
subtitle: Slack ChatBot
gh-repo: daattali/beautiful-jekyll
gh-badge: [star, fork, follow]
tags: [SSAFY]
comments: true
---

 SSAFY_9반_이한솔_https://github.com/onenumbersol/SSAFY/blob/master/2018_12_21_chatbot
 SSAFY 2주차 과제로 Python을 활용한 나만의 챗봇을 만들었다. 나는 조성우, 황유성과 함께 LOL Chat Bot을 만들었다.
 
---

## 1.스펙(Specification)  
(1) 사용자의 커멘드를 통해 챗봇에게 명령을 내리고 데이터를 분석한다
- 커멘드는 _(언더바)를 통해 구분한다 ex) @summoners_command_username
- 커멘드를 통해 명령을 구분하고, 데이터는 op.gg 사이트를 통해 가져온다
(2) 기능 소개
- Help : 봇과 소통할 수 있는 양식과 명령어 소개
- 기본 정보 제공 : 현재 티어 / 리그 포인트 / 승, 패 / 현재 속한 리그
- 전 시즌 티어 정보 : 현재까지 거쳐온 리그의 티어 정보 제공
- 현재 시즌 모스트 5 챔피언 : 프리시즌 기간 중 가장 많이 플레이 한 챔프 / 평균 CS와 분당 CS를 제공
- 최근 7일간 랭크 승률 : 7일간의 게임 결과를 추출하여 최근 승률을 제공

---

## 2. 회고(Retrospective)
(1) 어플리케이션 구현 과정에서의 어려움

- 사용자의 아이디를 직접 입력받아 검색하였기 때문에 인코딩이 필요하였다.
- 같은 정보임에도 Class의 이름이 달라 검색에 어려움이 있었다.
- 소환사마다 플레이 정보가 다르기 때문에 크롤링에 어려움이 있었다.


(2) 어플리케이션 구현 과정에서의 문제점

- Beautiful soup의 기술적인 한계가 있었다.
- 파이썬 초급 단계였기 때문에 코딩과정에서 구조적인 면이 부족했다.

---

## 3. 보완 계획(Feedback)

- 크롤링 한 데이터를 토대로 새로운 정보를 생성한다.
- 현재 플레이하고 있는 게임 정보를 출력한다.
- 코드를 간소화하고 구조화한다.
- Selenium을 사용하여 버튼 이벤트를 통한 크롤링을 구현한다.
- 자주 사용하는 대화 앱인 디스코드로 이식한다.
