# JUST-PLAN 프로젝트 목차
1. [프로젝트 소개](#프로젝트-소개)
2. [시스템 아키텍처](#시스템-아키텍처)
3. [기술 스택](#TECH-STACKS)
5. [문서화](#문서)
5. [기능 소개](#기능-소개)
6. [팀 소개](#팀-소개)



# JUST-PLAN
<div align="center"><img src="https://github.com/Break-it-all/.github/assets/83001865/abec01cb-b132-4801-8c92-0eb096699345"></div>

## 프로젝트 소개
Bita 서비스는 음성 채팅 구현을 위한 WebRtc와 CRDT 구현을 위한 WebSocket을 활용하여 페어프로그래밍과 멀티프로그래밍을 웹사이트에서 진행할 수 있도록 구현한 웹 IDE 서비스입니다.

## 시스템 아키텍처
환경 문제로 생기는 에러를 방지하기위해 docker-compose를 미리 셋팅하여 개발하였고, 웹 서버 라우팅 기능을 위해 nginx를 사용했습니다.


프론트엔드 개발 시 사용한 기술스택으로는 react, 컴파일 단에서 타입 에러를 방지하기 위한 typescript, react 상태 관리를 편하게 하기 위한 redux, css프레임워크로 tailwindcss를 사용하였습니다.


코드 컴파일 오픈 소스인 CodeX를 사용하여 컴파일 기능을 구현했고, 코드 저장하는 용도로 S3를 사용했습니다.


사용자 정보를 빠르게 조회할 수 있도록 redis에 refresh-token을 저장했습니다.

<div align="center"><img src="https://github.com/Break-it-all/.github/assets/83001865/326d8bea-7cd3-485f-bbf9-b94daf6e13cc"></div>


## TECH-STACKS

|Frontend|Backend|Database&Storage|DevOps| 
| :----: | :---: |   :---------:  | :--: |
|<img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=React&logoColor=white"><br><img src="https://img.shields.io/badge/Redux-764ABC?style=for-the-badge&logo=Redux&logoColor=white"><br><img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=TypeScript&logoColor=white"><br><img src="https://img.shields.io/badge/Tailwind CSS-06B6D4?style=for-the-badge&logo=Tailwind CSS&logoColor=white"><br>|<img src="https://img.shields.io/badge/Java-007396?style=for-the-badge&logo=Java&logoColor=white"><br><img src="https://img.shields.io/badge/Spring-37814A?style=for-the-badge&logo=Spring&logoColor=white"><br><img src="https://img.shields.io/badge/SpringBoot-85EA2D.svg?style=for-the-badge&logo=SpringBoot&logoColor=white"><br><img src="https://img.shields.io/badge/Swagger-38B832.svg?style=for-the-badge&logo=Swagger&logoColor=white">|<img src="https://img.shields.io/badge/mysql-4479A1?style=for-the-badge&logo=mysql&logoColor=white"><br><img src="https://img.shields.io/badge/Amazon RDS-527FFF?style=for-the-badge&logo=Amazon RDS&logoColor=white"><br>|<img src="https://img.shields.io/badge/Amazon EC2 -FF9900?style=for-the-badge&logo=Amazon EC2&logoColor=white"><br><img src="https://img.shields.io/badge/Amazon S3-569A31?style=for-the-badge&logo=Amazon S3&logoColor=white"><br> |


## 문서

### Linear

부족한 개발 기간으로 Github-flow 브랜치 전략를 사용해서 협업하고 JIRA를 사용해서 1주단위로 스프린트를 관리했습니다.

<div align="center"><img src="https://github.com/Break-it-all/.github/assets/83001865/b8bf501b-a6a1-4db5-8f35-2492cbedeed4"></div>

### 피그마
<div align="center"><img src="https://github.com/Break-it-all/.github/assets/83001865/bae58273-aad2-4683-9e18-d4cfc52ff8ea"></div>

### ERD
<div align="center"><img src="https://github.com/Break-it-all/.github/assets/83001865/b8343992-ddf9-4957-9e2a-e42a53757f7b"></div>

### API 문서화
<div align="center"><img src="https://github.com/Break-it-all/.github/assets/83001865/46791c0d-bc6d-45eb-8469-14b175402224"></div>
<div align="center"><img src="https://github.com/Break-it-all/.github/assets/83001865/06f417fa-7eaf-4462-b15d-43f4387457ca"></div>


## 기능 소개

![가계부](https://github.com/Just-Plan/.github/assets/83001865/3c82fbac-647a-45e8-a134-cca7f9149e1b)
![드래그앤드롭](https://github.com/Just-Plan/.github/assets/83001865/3068f627-1682-4983-9e94-0ced06821c74)
![마이페이지](https://github.com/Just-Plan/.github/assets/83001865/8a40a88c-7c5d-4c4c-a8e9-0eb034e6137b)
![메인페이지필터링](https://github.com/Just-Plan/.github/assets/83001865/3a325094-9218-4e9c-aad1-c11a27d87eae)
![일정 가져오기](https://github.com/Just-Plan/.github/assets/83001865/438288d3-0202-4e3e-a5a1-8091a3593c2c)
![메모,장소상세](https://github.com/Just-Plan/.github/assets/83001865/5181d5e2-44f7-4e49-ae02-ae7e793e1ab6)
![장소생성](https://github.com/Just-Plan/.github/assets/83001865/f0a8cdc6-afe9-440c-8aa1-c9f1b6572b2b)
![플랜생성](https://github.com/Just-Plan/.github/assets/83001865/2ef51305-968b-4de2-af4f-0f8bb81a4112)
![회원가입_로그인](https://github.com/Just-Plan/.github/assets/83001865/8fa4a73d-43b0-4d39-bb6c-3e0d368a0526)
![mbti테스트](https://github.com/Just-Plan/.github/assets/83001865/c75e78b8-4bd1-42d3-babb-ed35ab2a6d67)


### 회원가입/로그인
회원가입
- 가입을 수행할 이메일을 입력받은 후, Gmail에서 제공하는 SMTP 서버를 이용하여 해당 이메일로 인증 메일을 발송합니다.
- 메일에 포함된 URL에 접속하여 인증을 마친 뒤, 입력된 회원정보를 기반으로 회원가입이 수행됩니다.

로그인

- 이메일과 비밀번호를 입력받아 로그인을 수행합니다.
- 존재하지 않는 이메일을 입력하거나, 틀린 비밀번호를 입력할 시 경고 문구를 띄웁니다.
<div align="center"><img src="https://github.com/Break-it-all/.github/assets/83001865/4f8529f1-4cdd-4151-90f1-e859619ebc13"></div>

### 컨테이너 CRUD
코드를 편집할 수 있는 컨테이너를 생성합니다. 컨테이너 생성 시 이름, 설명, 언어, 모드를 선택할 수 있습니다.


컨테이너 이름은 ...버튼을 눌러 수정할 수 있으며 컨테이너 삭제도 가능합니다.


내 컨테이너는 내가 만든 컨테이너, 공유된 컨테이너는 상대방이 초대한 컨테이너가 보입니다.
<div align="center"><img src="https://github.com/Break-it-all/.github/assets/83001865/efa74aa5-0f03-4213-ab5e-101aa5f5bd57"></div>

### 페어 프로그래밍
페어 프로그래밍 네비게이터와 드라이버가 서로 음성 채팅을 통하여 소통하며 코드를 수정하는 모드 입니다. 


우측 상단에 버튼을 통하여 드라이버와 네비게이터를 변경하며 진행할 수 있습니다.
<div align="center"><img src="https://github.com/Break-it-all/.github/assets/83001865/648f10d0-ee18-49e8-86c7-d1e8e8bc917c"></div>

### 멀티 프로그래밍
멀티 프로그래밍 여러명의 사용자가 한 컨테이너에 접속하여 코드를 동시편집할 수 있는 모드입니다.


편집하는 사용자는 위쪽에 이름이 표시됩니다.
<div align="center"><img src="https://github.com/Break-it-all/.github/assets/83001865/524ca670-e3ce-4752-9cea-4317e8b862eb"></div>
위 두개의 모드는 컴파일을 통하여 에러나 코드 결과를 아래쪽에 출력해줍니다.

### 음성 채팅
WebRTC (Web Real-Time Communication)는 웹 브라우저 간에 플러그인의 도움 없이 서로 통신할 수 있도록 설계된 API입니다.


WebRTC 이용을 위해 시그널링 서버를 구현하여 SDP(서로의 음성,영상, 비디오 등 스트리밍 규약을 맞추는 과정), ICE(서로 통신 할 수 있는 최적의 경로를 찾을 수 있도록 도움)등의 정보를 교환합니다.


저희는 이러한 WebRTC를 이용하여 음성 채팅을 구현하였습니다.
<div align="center"><img src="https://github.com/Break-it-all/.github/assets/83001865/41466533-25ae-4fb0-913e-f636a4d50f7a"></div>




## 팀 소개

<table width="500" align="center">
<tbody>
<tr>
<th>Pictures</th>
<td width="100" align="center">
<a href="https://github.com/choiminwoo98">
<img src="https://avatars.githubusercontent.com/u/61531483?v=4" width="60" height="60">
</a>
</td>
<td width="100" align="center">
<a href="https://github.com/rnignon">
<img src="https://avatars.githubusercontent.com/u/86004439?v=4" width="60" height="60">
</a>
</td>
<td width="100" align="center">
<a href="https://github.com/wlstnam">
<img src="https://avatars.githubusercontent.com/u/127458907?v=4" width="60" height="60">
</a>
</td>
<td width="100" align="center">
<a href="https://github.com/hstla">
<img src="https://user-images.githubusercontent.com/97827316/215991535-aa0d5aeb-363c-41a7-a114-c1448d58d9f1.png"" width="60" height="60">
</a>
</td>
</tr>
<tr>
<th>Name</th>
<td width="100" align="center">최민우</td>
<td width="100" align="center">김민형</td>
<td width="100" align="center">남진수</td>
<td width="100" align="center">황현성</td>
</tr>
<tr>
<th>Position</th>
<td width="150" align="center">
Frontend<br>
</td>
<td width="150" align="center">
Frontend Backend<br>
</td>
<td width="150" align="center">
Frontend Backend<br>
</td>
<td width="150" align="center">
Frontend Backend<br>
</td>
</tr>
<tr>
<th>GitHub</th>
<td width="100" align="center">
<a href="https://github.com/choiminwoo98">
<img src="http://img.shields.io/badge/choiminwoo98-green?style=social&logo=github"/>
</a>
</td>
<td width="100" align="center">
<a href="https://github.com/rnignon">
<img src="http://img.shields.io/badge/rnignon-green?style=social&logo=github"/>
</a>
</td>
<td width="100" align="center">
<a href="https://github.com/wlstnam">
<img src="http://img.shields.io/badge/wlstnam-green?style=social&logo=github"/>
</a>
</td>
<td width="100" align="center">
<a href="https://github.com/hstla">
<img src="http://img.shields.io/badge/hstla-green?style=social&logo=github"/>
</a>
</td>
</tr>
</tbody>
</table>

