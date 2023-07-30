---
title: Project
permalink: /project/
layout: page
excerpt: 
comments: true
---

<style>
.project {
    font-size: 0;
}
.project > dl {
    display: inline-block;
    vertical-align: top;
    margin-top: 5rem;
    width: 45%;
    font-size: 1rem;
}
.project > dl:nth-child(2n) {
    padding-left: 10%;
}
.project > dl dt {
    position: relative;
    padding-left: 4rem;
    font-weight: bold;
}
.project > dl dt img {
    position: absolute;
    top: 50%;
    left: 0.5rem;
    transform: translateY(-50%);
    width: 2.5rem;
}
.project > dl .title {
  font-weight: bold;
}
.project > dl .date {
    line-height: 1.3rem;
    font-size: 0.8rem;
    font-weight: normal;
    opacity: 0.8;
}
.project > dl .info {
    margin-top: 1rem;
    word-break: break-all;
}
.project > dl .service {
  margin-top: 1.5rem;
}
.project > dl .service dt {
    padding-left: 0;
}
.project > dl .service dd {
    position: relative;
    padding-left: 1rem;
}
.project > dl .service dd:before {
    content: '·';
    position: absolute;
    top: 0;
    left: 0.3rem;
}
.project > dl .skill {
  margin-top: 1.5rem;
}
.project > dl .skill dt {
  padding-left: 0;
}
.project > dl .skill p {
  position: relative;
  margin: 5px 0;
  padding-left: 80px;
  line-height: 24px;
}
/* .project > dl .skill p.back-end span {
  opacity: 0.3;
} */
.project > dl .skill p strong {
  position: absolute;
  top: 0;
  left: 0;
  font-weight: bold;
}
.project > dl .skill p span {
  display: inline-block;
  margin-right: 2px;
  border-radius: 3px;
  padding: 0 5px;
  line-height: 20px;
  font-size: 13px;
}
.project > dl .skill p span.javascript {
  background-color: #fac651;
  color: #fff;
}
.project > dl .skill p span.react {
  background-color: #5fd3f3;
  color: #fff;
}
.project > dl .skill p span.redux {
  background-color: #7248b6;
  color: #fff;
}
.project > dl .skill p span.node {
  background-color: #7fc728;
  color: #fff;
}
.project > dl .skill p span.express {
  background-color: #7fc728;
  color: #fff;
}
.project > dl .skill p span.mysql {
  background-color: #dd8a00;
  color: #fff;
}
.project > dl .skill p span.jest {
  background-color: #944058;
  color: #fff;
}
.project > dl .skill p span.aws {
  background-color: #ff9900;
  color: #fff;
}
.project > dl .skill p span.git {
  background-color: #f05030;
  color: #fff;
}
.project > dl .skill p span.notion {
  background-color: #000;
  color: #fff;
}
.project > dl .skill p span.slack {
  background-color: #d91d57;
  color: #fff;
}
.project > dl .skill p span.trello {
  background-color: #2580f7;
  color: #fff;
}
.project > dl .skill p span.sass {
  background-color: #c76395;
  color: #fff;
}
.project > dl .skill p span.react-router {
  background-color: #5fd3f3;
  color: #fff;
}
.project > dl .skill p span.vercel {
  background-color: #000;
  color: #fff;
}
.project > dl .skill p span.typescript {
  background-color: #2f74c0;
  color: #fff;
}
.project > dl .skill p span.styled-components {
  background-color: #d3896e;
  color: #fff;
}
.project > dl .skill p span.react-query {
  background-color: #f73f51;
  color: #fff;
}
.project > dl .skill p span.recharts {
  background-color: #20afb9;
  color: #fff;
}
.project > dl .link {
    margin-top: 0.5rem;
    text-align: center;
    font-size: 0;
}
.project > dl .link a {
    text-decoration: none;
    font-weight: bold;
    font-size: 0.8rem;
    color: #333;
}
.project > dl .link a:after {
    content: '';
    position: relative;
    top: 0.1rem;
    display: inline-block;
    margin: 0 0.3rem;
    width: 1px;
    height: 0.7rem;
    background-color: #ccc;
}
.project > dl .link a:last-child:after {
    display: none;
}
.project > dl .img {
    display: block;
    position: relative;
    overflow: hidden;
    margin-top: 1rem;
    border-radius: 10px;
    box-shadow: 0 0 4px rgba(0, 0, 0, 0.2);
}
.project > dl .img::after  {
    display: none;
}
.project > dl .img img {
  transition: 0.2s;
}
.project > dl .img:hover img {
  transform: scale(1.05);
}


@media all and (max-width: 500px) {
    .project > dl {
        width: 100%;
    }
    .project > dl:nth-child(2n) {
        padding: 0;
    }
}
</style>

  <div class="project">
    <dl>
      <dt>
        <img src="/assets/img/logo-airbnb.png" alt="airbnb logo" />
        <div class="title"><strong>Airbnb를 모티브로한 팀 프로젝트</strong></div>
        <div class="date">2022.08.29 ~ 2022.09.08</div>
        <div class="date">주관 : 위코드 부트캠프</div>
      </dt>
      <dd>
        <a href="https://www.youtube.com/watch?v=DWaKFjUI7Ew" target="_blank" class="img">
          <img src="/assets/img/project-wenb.png" alt="wenb 프로젝트 영상" />
        </a>
        <div class="link">
          <a href="https://www.youtube.com/watch?v=DWaKFjUI7Ew" target="_blank" >배포 영상</a>
          <a href="https://bitnaleeeee.github.io/wecode-2st-project/" target="_blank">회고록</a>
          <a href="https://github.com/bitnaleeeee/36-2nd-WeNB-frontend" target="_blank">GitHub</a>
        </div>
        <div class="info">숙박 공유 서비스 Airbnb의 클론코딩이며 두번째 프로젝트인 만큼 1차 프로젝트의 아쉬웠던 부분을 보완하며 작업하게 되었습니다. 위 프로젝트는 유저 페이지와 호스트 페이지가 나눠져있어 기능적으로 구현할 부분이 많아 학습에 도움이 많이 되었습니다.</div>
        <dl class="service">
          <dt><strong>주요 기능</strong></dt>
          <dd>반응형 웹, 케럿셀, 아코디언 메뉴 적용</dd>
          <dd>리뷰 평점 분포 그래프 적용</dd>
          <dd>평점 표현시 소수 한자리 반올림 적용</dd>
          <dd>쿼리파라미터를 이용한 페이지네이션 구현</dd>
          <dd>네이버 맵 라이브러리 및 파일첨부 적용</dd>
        </dl>
        <dl class="skill">
          <dt><strong>기술 스택</strong></dt>
          <dd>
            <p class="front-end">
              <strong>Front-End</strong>
              <span class="react">React</span>
              <span class="javascript">JavaScript</span>
              <span class="redux">Redux</span>
            </p>
            <p class="back-end">
              <strong>Back-End</strong> 
              <span class="node">Node.js</span>
              <span class="express">Express</span>
              <span class="mysql">MySQL</span>
              <span class="jest">JEST</span>
              <span class="aws">AWS(EC2)</span>
            </p>
            <p class="tool">
              <strong>Tool</strong>
              <span class="git">Git</span>
              <span class="notion">Notion</span>
              <span class="slack">Slack</span>
              <span class="trello">Trello</span>
            </p>
          </dd>
        </dl>
      </dd>
    </dl>
    <dl>
      <dt>
        <img src="/assets/img/logo-aesop.png" alt="aesop logo" />
        <div class="title"><strong>Aesop을 모티브로한 팀 프로젝트</strong></div>
        <div class="date">2022.08.12 ~ 2022.8.26</div>
        <div class="date">주관 : 위코드 부트캠프</div>
      </dt>
      <dd>
        <a href="https://www.youtube.com/watch?v=n2kL24FnHsE" target="_blank" class="img">
          <img src="/assets/img/project-usopp.png" alt="우솝 프로젝트 영상" />
        </a>
        <div class="link">
          <a href="https://www.youtube.com/watch?v=n2kL24FnHsE" target="_blank" >배포 영상</a>
          <a href="https://bitnaleeeee.github.io/wecode-1st-project/" target="_blank">회고록</a>
          <a href="https://github.com/bitnaleeeee/36-1st-Usopp-frontend" target="_blank">GitHub</a>
        </div>
        <div class="info">커머스 사이트 Aesop을 모티브로 제작한 클론코딩 프로젝트 입니다. 첫 프로젝트인 만큼 서버에서 넘어오는 데이터를 어떻게 UI에 뿌려줄지 고민하며 겪은 시행착오 과정이 큰 경험이 되었습니다. 또한 팀원들과 협업하면서 효율적인 업무를 위한 커뮤니케이션의 중요성을 다시끔 깨달았습니다.</div>
        <dl class="service">
          <dt><strong>주요 기능</strong></dt>
          <dd>로그인폼 유효성 검사 함수에 따른 화면 구현</dd>
          <dd>이메일 정보를 호출하여 DB에 없다면 메세지 출력과 회원가입으로 이동</dd>
          <dd>이메일 정보 일치시 패스워드 입력란 호버 출력</dd>
          <dd>정규식에 맞는 ID/PW 일치시 계정생성</dd>
          <dd>장바구니에 상품 담기, 삭제, 수량 조절 구현</dd>
        </dl>
        <dl class="skill">
          <dt><strong>기술 스택</strong></dt>
          <dd>
            <p class="front-end">
              <strong>Front-End</strong>
              <span class="react">React</span>
              <span class="javascript">JavaScript</span>
              <span class="redux">Redux</span>
            </p>
            <p class="back-end">
              <strong>Back-End</strong> 
              <span class="node">Node.js</span>
              <span class="express">Express</span>
              <span class="mysql">MySQL</span>
              <span class="jest">JEST</span>
              <span class="aws">AWS(EC2)</span>
            </p>
            <p class="tool">
              <strong>Tool</strong>
              <span class="git">Git</span>
              <span class="notion">Notion</span>
              <span class="slack">Slack</span>
              <span class="trello">Trello</span>
            </p>
          </dd>
        </dl>
      </dd>
    </dl>
    <dl>
      <dt>
        <img src="/assets/img/logo-house.png" alt="github logo" />
        <div class="title"><strong>오늘의집 모바일 페이지 클론코딩</strong></div>
        <div class="date">2023.07.20 ~ 2023.07.30</div>
      </dt>
      <dd>
        <a href="https://clone-house.vercel.app/" target="_blank" class="img">
          <img src="/assets/img/project-house.png" alt="오늘의집 모바일 메인 페이지 클론코딩" />
        </a>
        <div class="link">
          <a href="https://clone-house.vercel.app/" target="_blank">배포 링크</a>
          <a href="https://github.com/bitnaleeeee/clone-house" target="_blank">GitHub</a>
        </div>
        <div class="info">오늘의집 사이트 모바일 버전을 클론코딩 하였습니다. 실제 서비스되는 화면과 최대한 비슷하게 작업하였습니다. 각 데이터 포멧에 맞게 UI 구성을 하였으며, 재활용성에 용이하도록 컴포넌트 구성을 하고 있습니다.(작업중)</div>
        <dl class="service">
          <dt><strong>주요 기능</strong></dt>
          <dd>첫 안내 모달팝업 24시간 뒤 재오픈 기능</dd>
          <dd>슬라이드 배너(추가중)</dd>
        </dl>
        <dl class="skill">
          <dt><strong>기술 스택</strong></dt>
          <dd>
            <p class="front-end">
              <strong>Front-End</strong>
              <span class="react">React</span>
              <span class="javascript">JavaScript</span>
              <span class="sass">SASS</span>
              <span class="react-router">React Router</span>
            </p>
            <p class="back-end">
              <strong>Back-End</strong> 
              <span class="vercel">Vercel</span>
            </p>
            <p class="tool">
              <strong>Tool</strong>
              <span class="git">Git</span>
            </p>
          </dd>
        </dl>
      </dd>
    </dl>
    <dl>
      <dt>
        <img src="/assets/img/logo-naver.png" alt="github logo" />
        <div class="title"><strong>네이버 모바일 페이지 클론코딩</strong></div>
        <div class="date">2023.06.12 ~ 2023.06.17</div>
      </dt>
      <dd>
        <a href="https://clone-naver.vercel.app/" target="_blank" class="img">
          <img src="/assets/img/project-naver.png" alt="네이버 모바일 메인 페이지 클론코딩" />
        </a>
        <div class="link">
          <a href="https://clone-naver.vercel.app/" target="_blank">배포 링크</a>
          <a href="https://github.com/bitnaleeeee/clone-naver" target="_blank">GitHub</a>
        </div>
        <div class="info">포털사이트 네이버 모바일 버전을 클론코딩 하였습니다. 실제 서비스되는 화면과 최대한 비슷하게 작업하였으며, 스프라이프 기법 및 반응형 웹을 적용하였습니다. 현재는 네이버 검색폼 클릭시 검색 팝업이 출력되며 이후 네이버 검색 API를 활용하여 연관검색어 및 마이페이지 추가 기능을 구현 예정에 있습니다.</div>
        <dl class="service">
          <dt><strong>주요 기능</strong></dt>
          <dd>스프라이프 기법을 활용한 로딩속도 개선 및 웹 접근성 준수</dd>
          <dd>미디어 쿼리를 활용한 반응형 웹 구현</dd>
          <dd>네이버 검색 API를 활용한 연관검색어 기능(개발중)</dd>
          <dd>마이페이지 구현(개발중)</dd>
        </dl>
        <dl class="skill">
          <dt><strong>기술 스택</strong></dt>
          <dd>
            <p class="front-end">
              <strong>Front-End</strong>
              <span class="react">React</span>
              <span class="javascript">JavaScript</span>
              <span class="sass">SASS</span>
              <span class="react-router">React Router</span>
            </p>
            <p class="back-end">
              <strong>Back-End</strong> 
              <span class="vercel">Vercel</span>
            </p>
            <p class="tool">
              <strong>Tool</strong>
              <span class="git">Git</span>
            </p>
          </dd>
        </dl>
      </dd>
    </dl>
    <dl>
      <dt>
        <img src="/assets/img/logo-onboarding.png" alt="onboarding logo" />
        <div class="title"><strong>실시간 검색창 구축 및 Vercel 배포</strong></div>
        <div class="date">2022.08.12 ~ 2022.8.26</div>
      </dt>
      <dd>
        <a href="https://bitnaleeeee.github.io/medical-search/" target="_blank" class="img">
          <img src="/assets/img/project-search.png" alt="실시간 검색창 영상" />
        </a>
        <div class="link">
          <a href="https://bitnaleeeee.github.io/medical-search/" target="_blank" >배포 링크</a>
          <a href="https://bitnaleeeee.github.io/back-end-build/" target="_blank">관련 포스팅</a>
          <a href="https://github.com/bitnaleeeee/medical-search" target="_blank">GitHub</a>
        </div>
        <div class="info">프리온보딩 프로젝트중 하나로써 검색창에 질환명 검색시 실시간으로 API 호출 통해서 검색어를 추천해주는 UI를 구현하였습니다. 정규표현식/캐싱/리액트 최적화 등 여러가지 기술들을 경험 할 수 있었던 프로젝트입니다. 실시간으로 JSON Server를 동작하기 위해 Vercel에 직접 배포하는 과정도 기억에 남았습니다.</div>
        <dl class="service">
          <dt><strong>주요 기능</strong></dt>
          <dd>정규표현식을 사용하여 사용자가 검색한 텍스트와 일치하는 부분 볼드처리</dd>
          <dd>검색어가 없을 시 '검색어 없음' 표출</dd>
          <dd>API 호출 최적화(Debounce)</dd>
          <dd>키보드로 추천 검색어들 이동 가능하도록 구현</dd>
          <dd>캐싱 기능을 제공하는 라이브러리(React-Query)등을 사용 하지 않고 API 호출별로 로컬 캐싱 구현</dd>
          <dd>API 호출을 위한 JSON Server를 Vercel 서버에 배포</dd>
        </dl>
        <dl class="skill">
          <dt><strong>기술 스택</strong></dt>
          <dd>
            <p class="front-end">
              <strong>Front-End</strong>
              <span class="react">React</span>
              <span class="javascript">JavaScript</span>
              <span class="sass">SASS</span>
              <span class="react-router">React Router</span>
            </p>
            <p class="tool">
              <strong>Tool</strong>
              <span class="git">Git</span>
            </p>
          </dd>
        </dl>
      </dd>
    </dl>
    <dl>
      <dt>
        <img src="/assets/img/logo-wanted.png" alt="wanted logo" />
        <div class="title"><strong>로그인/회원가입, 투두 리스트</strong></div>
        <div class="date">2022.10.01 ~ 2022.10.07</div>
      </dt>
      <dd>
        <a href="https://wanted-pre-onboarding-frontend-bitna.vercel.app" target="_blank" class="img">
          <img src="/assets/img/project-todo.png" alt="원티드 프론트엔드코스 사전과제 영상" />
        </a>
        <div class="link">
          <a href="https://wanted-pre-onboarding-frontend-bitna.vercel.app" target="_blank">배포 링크</a>
          <a href="https://github.com/bitnaleeeee/wanted-pre-onboarding-frontend.git" target="_blank">GitHub</a>
        </div>
        <div class="info">원티드 프론트엔드코스 과정 선발 과제입니다. 로그인하여 토큰이 발급되면 TODO 페이지로 리다이렉트합니다. 글쓰기/수정/삭제 및 할일 상태를 서버와 POST 방식으로 통신을 구현하였습니다. 또한 로그인 유효성 검사/토큰 세션 저장 등 여러가지 로직을 경험할 수 있었습니다.</div>
        <dl class="service">
          <dt><strong>주요 기능</strong></dt>
          <dd>로그인, 회원가입 유효성 검사</dd>
          <dd>로그인 API 호출, 올바른 응답을 받았을 때 todo 경로로 이동</dd>
          <dd>로그인 여부에 따른 리다리렉트 처리 구현</dd>
          <dd>TODO 경로 접속시 투두 리스트, 입력창, 추가 버튼, 수정, 삭제 기능 구현</dd>
          <dd>TODO 체크 박스 구현</dd>
        </dl>
        <dl class="skill">
          <dt><strong>기술 스택</strong></dt>
          <dd>
            <p class="front-end">
              <strong>Front-End</strong>
              <span class="react">React</span>
              <span class="javascript">JavaScript</span>
              <span class="sass">SASS</span>
              <span class="react-router">React Router</span>
            </p>
            <p class="tool">
              <strong>Tool</strong>
              <span class="git">Git</span>
            </p>
          </dd>
        </dl>
      </dd>
    </dl>
    <dl>
      <dt>
        <img src="/assets/img/logo-github.png" alt="github logo" />
        <div class="title"><strong>GitHub 이슈 페이지 구축</strong></div>
        <div class="date">2022.10.29 ~ 2022.10.30</div>
      </dt>
      <dd>
        <a href="https://2nd-assignment.vercel.app/" target="_blank" class="img">
          <img src="/assets/img/project-issue.png" alt="원티드 프론트엔드코스 기업협업 과제" />
        </a>
        <div class="link">
          <a href="https://2nd-assignment.vercel.app/" target="_blank">배포 링크</a>
          <a href="https://github.com/bitnaleeeee/angular-cli-issue-list" target="_blank">GitHub</a>
        </div>
        <div class="info">특정 github(Angular-cli) 이슈 목록과 상세 내용을 확인하는 반응형 웹을 구현했습니다. GitHub REST API를 사용하여 access token발급받아 프론트엔드만으로 서버와 통신하고 웹을 구축하는 경험을 할 수 있었습니다.</div>
        <dl class="service">
          <dt><strong>주요 기능</strong></dt>
          <dd>지정조건에 맞게 데이터 요청 및 표시</dd>
          <dd>이슈 중 코멘트가 많은 순으로 정렬</dd>
          <dd>상세 이슈 페이지 구현</dd>
          <dd>화면을 아래로 스크롤 할 시 이슈 목록 추가 로딩(인피니티 스크롤)</dd>
          <dd>Context API를 활용한 이슈 상태관리 및 API 연동</dd>
        </dl>
        <dl class="skill">
          <dt><strong>기술 스택</strong></dt>
          <dd>
            <p class="front-end">
              <strong>Front-End</strong>
              <span class="react">React</span>
              <span class="javascript">JavaScript</span>
              <span class="typescript">TypeScript</span>
              <span class="styled-components">Styled-Component</span>
              <span class="react-router">React Router</span>
            </p>
            <p class="tool">
              <strong>Tool</strong>
              <span class="git">Git</span>
            </p>
          </dd>
        </dl>
      </dd>
    </dl>
    <dl>
      <dt>
        <img src="/assets/img/logo-onboarding.png" alt="onboarding logo" />
        <div class="title"><strong>차량대여 서비스 모바일 웹 제작</strong></div>
        <div class="date">2022.11.01 ~ 2022.11.03</div>
      </dt>
      <dd>
        <a href="https://3rd-assignment.vercel.app/" target="_blank" class="img">
          <img src="/assets/img/project-car.png" alt="원티드 프론트엔드코스 기업협업 과제" />
        </a>
        <div class="link">
          <a href="https://3rd-assignment.vercel.app/" target="_blank">배포 링크</a>
          <a href="https://github.com/bitnaleeeee/car-rental-service" target="_blank">GitHub</a>
        </div>
        <div class="info">Figma를 사용하여 디자인 및 B2C 차량 대여 서비스 모바일 웹을 그대로 제작한 프로젝트입니다. 쿼리키 값, 쿼리 함수에 대한 파라미터를 커스텀 훅으로 설정할 수 있게 분리하고 해당 페이지의 사용 맥락에 맞게 staleTime 옵션등을 활용해 사용성을 개선하였습니다.
        </div>
        <dl class="service">
          <dt><strong>주요 기능</strong></dt>
          <dd>Figma 상의 디자인 및 기능 구현</dd>
          <dd>차량 리스트: 차량이 없을 때 처리, 차량 불러오는 중 처리</dd>
          <dd>차량 상세 페이지 구현</dd>
          <dd> 카카오톡, 페이스북 공유 시 미리보기 기능</dd>
          <dd>비동기 통신 로직 최적화</dd>
        </dl>
        <dl class="skill">
          <dt><strong>기술 스택</strong></dt>
          <dd>
            <p class="front-end">
              <strong>Front-End</strong>
              <span class="react">React</span>
              <span class="javascript">JavaScript</span>
              <span class="typescript">TypeScript</span>
              <span class="styled-components">Styled-Component</span>
              <span class="react-query">React Query</span>
            </p>
            <p class="tool">
              <strong>Tool</strong>
              <span class="git">Git</span>
            </p>
          </dd>
        </dl>
      </dd>
    </dl>
    <dl>
      <dt>
        <img src="/assets/img/logo-onboarding.png" alt="onboarding logo" />
        <div class="title"><strong>B2C 투자서비스 관리자 패널 제작</strong></div>
        <div class="date">2022.11.12 ~ 2022.11.18</div>
      </dt>
      <dd>
        <a href="https://bitnaleeeee.github.io/investment-management/" target="_blank" class="img">
          <img src="/assets/img/project-investment-management.png" alt="B2C 투자 관리 서비스 영상" />
        </a>
        <div class="link">
          <a href="https://bitnaleeeee.github.io/investment-management/" target="_blank" >배포 링크</a>
          <a href="https://github.com/bitnaleeeee/investment-management" target="_blank">GitHub</a>
        </div>
        <div class="info">
          투자 관리 서비스의 관리자 페이지 리스트/상세 페이지를 구현하는 프로젝트입니다. 각 항목을 클릭하면 사용자의 상세 내역을 확인할 수 있으며 각 리스트는 페이지네비게이션을 적용하여 데이터를 추가로 불러오고 있습니다. 폼과 테이블은 Material-UI를 적용하였습니다. 데이터를 얻기 위해 JSON Server를 사용하다가 CORS 이슈가 있어 많은 시행착오를 겪으며 서버 로직을 수정했던 경험이 있었습니다.
        </div>
        <dl class="service">
          <dt><strong>주요 기능</strong></dt>
          <dd>계좌목록 데이터 조회 기능 구현</dd>
          <dd>페이지네이션 기능 구현</dd>
          <dd>계좌 목록 사용자 이름 클릭시 사용자 정보 조회</dd>
          <dd>사용자상세 데이터 조회</dd>
          <dd>사용자상세 페이지네이션</dd>
          <dd>로그인, 로그아웃</dd>
        </dl>
        <dl class="skill">
          <dt><strong>기술 스택</strong></dt>
          <dd>
            <p class="front-end">
              <strong>Front-End</strong>
              <span class="react">React</span>
              <span class="javascript">JavaScript</span>
              <span class="sass">SASS</span>
            </p>
            <p class="back-end">
              <strong>Back-End</strong> 
              <span class="node">Node.js</span>
              <span class="express">Express</span>
              <span class="aws">AWS(EC2)</span>
            </p>
            <p class="tool">
              <strong>Tool</strong>
              <span class="git">Git</span>
            </p>
          </dd>
        </dl>
      </dd>
    </dl>
    <dl>
      <dt>
        <img src="/assets/img/logo-onboarding.png" alt="onboarding logo" />
        <div class="title"><strong>광고현황 대시보드/관리 서비스</strong></div>
        <div class="date">2022.11.05 ~ 2022.11.06</div>
      </dt>
      <dd>
        <a href="https://frabjous-frangipane-831c63.netlify.app/" target="_blank" class="img">
          <img src="/assets/img/project-adlist.png" alt="광고현황 대시보드 영상" />
        </a>
        <div class="link">
          <a href="https://frabjous-frangipane-831c63.netlify.app/" target="_blank" >배포 링크</a>
          <a href="https://github.com/bitnaleeeee/ad-list" target="_blank">GitHub</a>
        </div>
        <div class="info">광고현황 대시보드를 리액트로 구현하는 프로젝트이며 디자인 산출물은 피그마로 전달받아 처음 사용하게 되었습니다. Recharts를 적용하면서 데이터 시각화 작업을 경험하였으며 Styled-Components를 사용하여 컴포넌트를 더욱 유연하게 사용하는 방법을 알게되었습니다.</div>
        <dl class="service">
          <dt><strong>주요 기능</strong></dt>
          <dd>대시보드 datePicker, 기간 필터</dd>
          <dd>대시보드 통합광고 현황</dd>
          <dd>대시보드 차트</dd>
          <dd>대시보드 지표별 필터</dd>
          <dd>페이지 이동시 상태유지</dd>
        </dl>
        <dl class="skill">
          <dt><strong>기술 스택</strong></dt>
          <dd>
            <p class="front-end">
              <strong>Front-End</strong>
              <span class="react">React</span>
              <span class="javascript">JavaScript</span>
              <span class="styled-components">Styled-Component</span>
              <span class="recharts">Recharts</span>
            </p>
            <p class="tool">
              <strong>Tool</strong>
              <span class="git">Git</span>
            </p>
          </dd>
        </dl>
      </dd>
    </dl>
  </div>