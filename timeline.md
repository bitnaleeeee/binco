---
title: Timeline
permalink: /timeline/
layout: page
excerpt: 
comments: true
---

<style>
.timeline {
  margin-top: 5rem;
}
.timeline > dl {
  position: relative;
  margin-top: 3rem;
  height: 12rem;
}
.timeline > dl:first-child {
  margin-top: 0;
}
.timeline > dl dt {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  border-radius: 50%;
  width: 7rem;
  height: 7rem;
  background-color: #ececec;
}
.timeline > dl dt img {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  box-sizing: border-box;
  padding: 1rem;
  width: 100%;
}
.timeline > dl dt::before {
  content: '';
  position: absolute;
  top: 0;
  left: 50%;
  z-index: -1;
  transform: translateX(-50%);
  border-left: 5px dotted #ececec;
  height: 15rem;
}
.timeline > dl dd {
  position: absolute;
  top: 50%;
  left: 0;
  transform: translateY(-50%);
  width: 37%;
  text-align: left;
}
.timeline > dl dd .date {
  line-height: 1.3;
  font-size: 0.8rem;
  opacity: 0.8;
}
.timeline > dl dd .title {
  display: inline-block;
  line-height: 1.5;
}

.timeline > dl dd .title .dot {
  margin: 0 0.1rem;
  opacity: 0.3;
}
.timeline > dl dd .link {
  position: relative;
  display: inline-block;
  z-index: 10;
  text-decoration: none;
  font-weight: bold;
  color: #FE6672;
}
.timeline > dl dd .link:after {
  display: none;
}
.timeline > dl::after {
  content: '';
  display: block;
  clear: both;
}
.timeline > dl:nth-child(2n) dd {
  left: auto;
  right: 0;
  text-align: right;
}

.timeline > dl:last-child dt:before {
  display: none;
}
</style>

<div class="timeline">
  <dl>
    <dt>
      <img src="/assets/img/logo-frontend.png" alt="onboarding logo" />
    </dt>
    <dd>
      <strong class="title">원티드 프론트엔드 코스</strong>
      <!-- <div class="date">2022.10 - 2022.11</div> -->
      <p class="text">원티드에서 주관하는 프론트엔드 챌린지이며, 막판 스퍼트가 필요한 주니어를 위해 2주간 집중 학습하는 경험을 하였습니다.</p>
    </dd>
  </dl>
  <dl>
    <dt>
      <img src="/assets/img/logo-onboarding.png" alt="onboarding logo" />
    </dt>
    <dd>
      <strong class="title">원티드 프리온보딩 코스</strong>
      <!-- <div class="date">2022.10 - 2022.11</div> -->
      <p class="text">원티드에서 주관하는 프론트엔드 코스(Pre-On Boarding)로써 여러 IT기업의 실무 과제로 이루어졌으며 실무자/취준생 등 여러 팀원들과 같이 다양한 프로젝트를 진행하였습니다.</p>
    </dd>
  </dl>
  <dl>
    <dt>
      <img src="/assets/img/logo-weggle.png" alt="weggle logo" />
    </dt>
    <dd>
      <strong class="title">위글 기업 인턴십</strong>
      <!-- <div class="date">2022.09 - 2022.10</div> -->
      <p class="text">부트캠프 기업 협업 인턴쉽으로 숏폼커머스 플랫폼 위글에서 백 오피스 프로젝트를 진행하면서 실무 로직 및 가이드를 경험하였습니다.</p>
    </dd>
  </dl>
  <dl>
    <dt>
      <img src="/assets/img/logo-wecode.png" alt="wecode logo" />
    </dt>
    <dd>
      <strong class="title">위코드 부트캠프</strong>
      <!-- <div class="date">2022.06 ~ 2022.10</div> -->
      <p class="text">프론트엔드 개발자로 나아가고 다양한 프로젝트를 경험하기 위해 위코드 부트캠프를 수료하였습니다. 웹에 대한 폭넓은 학습 및 알고리즘을 학습했으며, 프론트/서버 개발자와 다양한 프로젝트를 진행하면서 많은 경험을 쌓았습니다.</p>
    </dd>
  </dl>
  <dl>
    <dt>
      <img src="/assets/img/logo-codeit.png" alt="codeit logo" />
    </dt>
    <dd>
      <strong class="title">코드잇 프론트엔드 과정</strong>
      <!-- <div class="date">2022.03 ~ 2022.06</div> -->
      <p class="text">생활코딩 강의를 시작으로 HTML, CSS, JavaScript를 학습하였으며 체계적으로 배우기위해 코드잇 프론트엔드 과정을 수강하였습니다. 단순히 학습하는것이 아닌 다양한 UI를 구축해보면서 개발의 매력에 더욱 빠지게 되었습니다.<br /><a href="https://codepen.io/bitnaleeeee/" target="_blank" class="link">UI 보러가기</a>
      </p>
    </dd>
  </dl>
  <dl>
    <dt>
      <img src="/assets/img/logo-yogiyo.png" alt="yogiyo logo" />
    </dt>
    <dd>
      <strong class="title">위대한상상<span class="dot">·</span>경희대학교<span class="dot">·</span>화성고등학교</strong>
      <!-- <div class="date">2018.02 ~ 2022.02</div> -->
      <p class="text">인사, HRD 업무 담당하였으며 IT부서에서 일하면서 웹 개발에 대한 관심이 생겼고 이때부터 개발자의 커리어 전환에 도전하게 되었습니다.</p>
    </dd>
  </dl>
</div>