# JUST-PLAN 프로젝트 목차
1. [프로젝트 소개](#프로젝트-소개)
2. [시스템 아키텍처](#시스템-아키텍처)
3. [기술 스택](#TECH-STACKS)
5. [문서화](#문서)
5. [기능 소개](#기능-소개)
6. [팀 소개](#팀-소개)



# JUST-PLAN
<div align="center"><img src="https://github.com/Break-it-all/frontend/assets/83001865/19b92afd-044e-4ca4-abcd-58410943ae36"></div>

## 프로젝트 소개
다른 사람의 검증된 여행 일정을 가져와 자신만의 여행 일정으로 손쉽게 작성할 수 있는 여행 일정 플래너입니다.

MBTI와 지역 필터링으로 사용자 맞춤 여행 일정을 제공하며, 장소마다 방문한 사용자의 MBTI 통계를 볼 수 있어 자신의 취향에 맞는 여행 장소를 선택할 수 있습니다.



## 시스템 아키텍처
환경 문제로 생기는 에러를 방지하기 위해 docker-compose를 미리 셋팅하여 개발하였고, 웹 서버 리버스 프록시 역할과 보안 강화를 nginx와 certbot를 사용하여 구현하였습니다.

프론트엔드 개발 시 사용한 기술 스택으로는 Next.js 14, 컴파일 단에서 타입 에러를 방지하기 위한 typescript, 전역 상태 관리를 편하게 하기 위한 jotai, 서버 상태 관리를 위한 react-query, css 프레임워크로 tailwindcss 및 공유 ui 컴포넌트인 shadcn/ui를 사용하였습니다. 지도 기능을 제공하기 위해 카카오 지도 api, google map api를 사용하였으며 드래그 앤 드랍을 위해 hello-pangea/dnd 라이브러리를 사용하였습니다.

RDS의 Mysql과 사용자 정보를 빠르게 조회할 수 있도록 redis에 refresh-token을 저장했고, swagger를 이용하여 API 문서화를 수행함으로써, 프론트엔드와의 협업을 용이하게 하였습니다.


<div align="center"><img src="https://github.com/Break-it-all/frontend/assets/83001865/dcf2c030-63c5-4758-bb5a-9df9681222cf"></div>
<br>


## TECH-STACKS

|Frontend|Backend|Database&Storage|DevOps| 
| :----: | :---: |   :---------:  | :--: |
|<img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=Next.js&logoColor=white"><br><img src="https://img.shields.io/badge/Jotai-764ABC?style=for-the-badge&logo=Jotai&logoColor=white"><br><img src="https://img.shields.io/badge/React_Query-FF4154?style=for-the-badge&logo=ReactQuery&logoColor=white"><br><img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=TypeScript&logoColor=white">|<img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white"><br><img src="https://img.shields.io/badge/Spring-37814A?style=for-the-badge&logo=Spring&logoColor=white"><br><img src="https://img.shields.io/badge/SpringBoot-85EA2D.svg?style=for-the-badge&logo=SpringBoot&logoColor=white"><br><img src="https://img.shields.io/badge/Swagger-38B832.svg?style=for-the-badge&logo=Swagger&logoColor=white">|<img src="https://img.shields.io/badge/mysql-4479A1?style=for-the-badge&logo=mysql&logoColor=white"><br><img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white"><br><img src="https://img.shields.io/badge/Amazon RDS-527FFF?style=for-the-badge&logo=Amazon RDS&logoColor=white"><br>|<img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=Docker&logoColor=white"/><br><img src="https://img.shields.io/badge/Amazon EC2 -FF9900?style=for-the-badge&logo=Amazon EC2&logoColor=white"><br><img src="https://img.shields.io/badge/Amazon S3-569A31?style=for-the-badge&logo=Amazon S3&logoColor=white"><br> |
<br>


## 문서

### **Linear**



<div align="center"><img src="https://github.com/Break-it-all/frontend/assets/83001865/ace69428-f05c-4e49-a7c4-11a36d4cb3b2"></div>
<p>부족한 개발 기간으로 Github-flow 브랜치 전략를 사용하여 협업을 수행하였고, Linear를 사용해서 1주 단위로 스프린트를 관리하였습니다.</p>
<br>

### **피그마**
<div align="center"><img width="946" alt="피그마 사진" src="https://github.com/Just-Plan/.github/assets/73208914/9474f283-6a6b-489c-92e4-7b708e777dd8"></div>
<br>

### **ERD**
<div align="center"><img src="https://github.com/Break-it-all/frontend/assets/83001865/386eb232-e01b-4bb8-a8cb-188a41e986ff"></div>
<br>

### **API 문서화**
<div align="center"><img src="https://github.com/Break-it-all/frontend/assets/83001865/aa93f3cd-4c70-4e5d-93a9-95dbca52555c"></div>
<p>프론트엔드와의 협업을 위해 swagger를 사용하여 API 문서화를 진행했습니다.</p>
<br>




## 기능 소개

### **회원가입/로그인**


<div align="center"><img src="https://github.com/Just-Plan/.github/assets/83001865/8fa4a73d-43b0-4d39-bb6c-3e0d368a0526">
<p>이메일 인증을 통한 회원가입을 제공하여 사용자를 인증하며, 회원 정보를 통해 회원/비회원 사용자 간의 접속할 수 있는 페이지를 구분하여 사용자에게 서비스를 제공합니다.</p>
</div>
<br>

### **mbti 테스트**

<div align="center"><img src="https://github.com/Just-Plan/.github/assets/83001865/c75e78b8-4bd1-42d3-babb-ed35ab2a6d67">
<p>사용자에게 잘 맞는 여행 플랜을 추천하고 장소의 MBTI 통계 정보를 제공하기 위해 사용자에게 여행 MBTI TEST를 실시하게 하여 사용자 맞춤 웹서비스를 제공합니다. </p>
</div>
<br>

### **메인페이지 필터링**

<div align="center"><img src="https://github.com/Just-Plan/.github/assets/83001865/3a325094-9218-4e9c-aad1-c11a27d87eae">
<p>"나의 여행 플랜 찾기"에서 지역을 선택하여, 이에 해당하는 일정을 필터링하여 조회할 수 있으며,</p>
<p>"MBTI 맞춤 여행 플랜"에서 MBTI를 선택하여, 해당 MBTI를 가진 작성자의 일정을 필터링하여 조회할 수 있습니다.</p></div>
<br>

### **일정 생성**

<div align="center"><img src="https://github.com/Just-Plan/.github/assets/83001865/2ef51305-968b-4de2-af4f-0f8bb81a4112">
<p>로그인이 되어있고, MBTI 테스트 결과가 존재한다면 일정 이름, 장소, 해시태그, 날짜 등을 작성하여 일정을 생성할 수 있습니다.</p>
</div>
<br>

### **장소 생성**

<div align="center"><img src="https://github.com/Just-Plan/.github/assets/83001865/f0a8cdc6-afe9-440c-8aa1-c9f1b6572b2b">
<p>"장소 추가하기" 버튼을 통해 장소를 추가할 수 있습니다.</p>
<p>장소 키워드를 검색하여 여행 지역 내의 장소를 조회할 수 있으며, 추가된 장소의 위치를 지도에서 확인할 수 있습니다.</p>
<p>장소를 클릭하여 장소에 대한 상세 정보를 확인할 수 있고, 다른 이용자가 작성한 댓글을 조회할 수 있습니다.</p>
</div>
<br>

### **일정 가져오기**

<div align="center"><img src="https://github.com/Just-Plan/.github/assets/83001865/438288d3-0202-4e3e-a5a1-8091a3593c2c">
<p>다른 사람의 검증된 일정을 가져오기 버튼을 통해 내 일정으로 만들 수 있습니다.</p>
<p>가져온 일정은 수정이 가능하여, 자신만의 일정으로 커스터마이징하여 손쉽게 일정을 만들 수 있습니다.</p>
</div>
<br>

### **일정 수정**

<div align="center"><img src="https://github.com/Just-Plan/.github/assets/83001865/3068f627-1682-4983-9e94-0ced06821c74">
<p>드래그 앤 드랍을 통해 사용자가 원하는 장소를 원하는 날짜에 추가 및 삭제하여 일정을 수정할 수 있습니다. </p>
<p>장소의 위치를 날짜에 맞게 추가 및 삭제할 수 있도록 사용자에게 맵을 제공합니다. </p>

</div>
<br>


### **가계부**

<div align="center"><img src="https://github.com/Just-Plan/.github/assets/83001865/3c82fbac-647a-45e8-a134-cca7f9149e1b">
<p>가계부를 ON/OFF 하여 작성할 수 있습니다.</p>
<p>현금, 카드를 구분하여 예산을 작성할 수 있으며, 교통, 음식, 쇼핑, 등의 카테고리 별로 지출 내역을 기록할 수 있습니다.</p>
</div>
<br>

### **메모, 장소 상세 페이지**

<div align="center"><img src="https://github.com/Just-Plan/.github/assets/83001865/5181d5e2-44f7-4e49-ae02-ae7e793e1ab6">
<p>장소에 대한 정보를 보여주거나 해당 장소에 많이간 MBTI 정보 그리고 댯글등을 사용자에게 제공합니다.장소별로 구매할 물품, 준비물같은 간단한 메모를 할 수 있습니다.</p>
<p>일정 내에 해당 장소가 있을 때는 메모를 추가하여 자신만의 정보들을 적어 놓을 수 있습니다.</p>
<p>장소 상세 페이지에서는 장소별 MBTI 통계, 댓글과 운영 시간을 확인할 수 있습니다.</p>
</div>
<br>


### **마이페이지**

<div align="center"><img src="https://github.com/Just-Plan/.github/assets/83001865/8a40a88c-7c5d-4c4c-a8e9-0eb034e6137b">
<p>사용자 정보를 토대로 관련된 여행 일정이나 가계부, 회원 정보 수정 기능을 제공합니다.</p>
</div>
<br>


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
<a href="https://github.com/dbswl701">
<img src="https://github.com/Just-Plan/.github/assets/73208914/5e265e35-77a7-4e65-ba11-09039ef33d16" width="60" height="60">
</a>
</td>
<td width="100" align="center">
<a href="https://github.com/rnignon">
<img src="https://avatars.githubusercontent.com/u/86004439?v=4" width="60" height="60">
</a>
</td>
<td width="100" align="center">
<a href="https://github.com/">
<img src="https://avatars.githubusercontent.com/u/142382002?v=4" width="60" height="60">
</a>
</td>
<td width="100" align="center">
<a href="https://github.com/hstla">
<img src="https://user-images.githubusercontent.com/97827316/215991535-aa0d5aeb-363c-41a7-a114-c1448d58d9f1.png" width="60" height="60">
</a>
</td>
</tr>
<tr>
<th>Name</th>
<td width="100" align="center">최민우</td>
<td width="100" align="center">강윤지</td>
<td width="100" align="center">김민형</td>
<td width="100" align="center">최윤정</td>
<td width="100" align="center">황현성</td>
</tr>
<tr>
<th>Position</th>
<td width="150" align="center">
Frontend<br>
</td>
<td width="150" align="center">
Frontend<br>
</td>
<td width="150" align="center">
Backend<br>
</td>
<td width="150" align="center">
Backend<br>
</td>
<td width="150" align="center">
Backend<br>
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
<a href="https://github.com/dbswl701">
<img src="http://img.shields.io/badge/choiminwoo98-green?style=social&logo=github"/>
</a>
</td>
<td width="100" align="center">
<a href="https://github.com/rnignon">
<img src="http://img.shields.io/badge/rnignon-green?style=social&logo=github"/>
</a>
</td>
<td width="100" align="center">
<a href="https://github.com/ChoiYoonJ">
<img src="http://img.shields.io/badge/ChoiYoonJ-green?style=social&logo=github"/>
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
