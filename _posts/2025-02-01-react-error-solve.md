---
layout: post
title: "리액트 전역 설치시 발생하는 에러 해결방법"
date: 2025-02-01 11:00:59
modified: 2025-02-01 11:00:59
tag: [React]

---

## 에러 발생
`create-react-app`을 사용하여 웹 애플리케이션을 만드려고 할때 발생한 에러와 해결방법에 대해 정리하고자 한다.

`npx crate-react-app cra-test` 를 터미널에 작성했을때 아래와 같은 에러가 발생하였다.

```javasciprt 
nstalling packages. This might take a couple of minutes.
Installing react, react-dom, and react-scripts with cra-template...

npm ERR! code EACCES
npm ERR! syscall link
npm ERR! path /Users/bitnalee/.npm/_cacache/tmp/a260a069
npm ERR! dest /Users/bitnalee/.npm/_cacache/content-v2/sha512/6d/fd/f467ed313b4bf4ab6153124f131511f89891b1f907288dc172884501b47aebd2de73de8457c0674632207600f8c8643b65cca67b7d0026f3900f2778f815
npm ERR! errno EACCES
npm ERR! 
npm ERR! Your cache folder contains root-owned files, due to a bug in
npm ERR! previous versions of npm which has since been addressed.
npm ERR! 
npm ERR! To permanently fix this problem, please run:
npm ERR!   sudo chown -R 501:20 "/Users/bitnalee/.npm"

npm ERR! A complete log of this run can be found in: /Users/bitnalee/.npm/_logs/2025-02-02T12_23_52_124Z-debug-0.log

Aborting installation.
  npm install --no-audit --save --save-exact --loglevel error react react-dom react-scripts cra-template has failed.

Deleting generated file... package.json
Deleting cra-test/ from /Users/bitnalee
Done.
```

### 원인
 해당 에러는 EACCES (Permission denied) 오류로, npm이 특정 폴더(~/.npm/ 캐시 폴더)에 대한 쓰기 권한이 없어서 발생한다.
따라서 설치 과정에서 권한 문제가 발생할 수 있으므로 
나의 경우 nvm(Node Version Manager)을 사용하여 Node.js를 설치하여 문제를 해결하였다.

### 해결방법
1. `nvm`설치
<p>
`curl -fsSL https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.4/install.sh | bash`


2. 환경변수 로드
<p>
`export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"
`

3. 최신 LTS 버전의 Node.js 설치
<p>
`nvm install --lts
nvm use --lts
`
후에 다시 create-react-app 을 사용하면 정상적으롷 웹 애플리케이션이 만들어지는 것을 확인할 수 있다. 