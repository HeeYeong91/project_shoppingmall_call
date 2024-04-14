# :eyeglasses: 안경 쇼핑몰 C-all
<br />

## :page_facing_up: 목차
1. 프로젝트 소개
2. 프로젝트 기능
   * [1. 메인 페이지 구현](#1-메인-페이지-구현)
   * [2. 회원가입 및 로그인 구현](#2-회원가입-및-로그인-구현)
   * [3. 제품 리스트 화면 구현](#3-제품-리스트-화면-구현)
   * [4. 제품 상세페이지 구현](#4-제품-상세페이지-구현)
   * [5. 리뷰 구현](#5-리뷰-구현)
   * [6. 매장 위치 카카오지도 API구현](#6-매장-위치-카카오지도-API구현)
   * [7. 장바구니 구현](#7-장바구니-구현)
   * [8. 주문 구현](#8-주문-구현) <br />
<br /><br />

## 맡은 개발 영역 <br />
4. 제품 상세페이지 구현 <br />
7. 장바구니 구현 <br />
<br />

## :eyes: 1. 프로젝트 소개
다이나믹 웹 프로젝트로 제작한 쇼핑몰 팀 프로젝트 <br />
MVC 패턴 연습을 위한 팀 프로젝트로 Model, View, Controller로 구분지어 구현 <br />
<br /><br />

자바 11버전, 다이나믹 웹 프로젝트 3버전, Tomcat 9버전 사용 <br />
깃허브에서 클론 후 이클립스로 실행하면 다이나믹 웹 프로젝트가 잘 실행이 안되기 때문에 <br />
깃허브에서 클론 진행 후 이클립스에서 따로 다이나믹 웹 프로젝트 생성 후 클론한 내용을 해당 프로젝트에 복사해서 사용 <br />
<br /><br />

데이터를 DB에서 저장 및 관리 <br />
src / main / java / config / jdbc.properties 에서 username에 SQLDeveloper 사용자 이름, password에 SQLDeveloper 비밀번호 입력 <br />
![jdbc설정파일](https://github.com/HeeYeong91/project_shoppingmall_call/assets/139057065/19c27383-4c2a-4cb5-bbc5-a5806722dc51) <br />
<br /><br />

:calendar: 프로젝트 기간 : 2023년 7월 24일 ~ 2023년 7월 28일 <br />
:hammer: Tools : ![Visual Studio Code](https://img.shields.io/badge/VS%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white) 
<img src="https://img.shields.io/badge/Eclipse-FE7A16.svg?style=for-the-badge&logo=Eclipse&logoColor=white" /> 
![Oracle](https://img.shields.io/badge/SQLDeveloper-F80000?style=for-the-badge&logoColor=white) <br /> 
:books: languages : ![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white) 
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E) ![Bootstrap](https://img.shields.io/badge/bootstrap-%238511FA.svg?style=for-the-badge&logo=bootstrap&logoColor=white) 
![Oracle](https://img.shields.io/badge/Oracle%20SQL-F80000?style=for-the-badge&logo=oracle&logoColor=white) ![Thymeleaf](https://img.shields.io/badge/Thymeleaf-%23005C0F.svg?style=for-the-badge&logo=Thymeleaf&logoColor=white) <br />
![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white) ![Java](https://img.shields.io/badge/JSP-%23ED8B00.svg?style=for-the-badge&logoColor=white) <br />
<br /> <br />

👨‍💻👩‍💻 멤버 구성
<table>
    <tr>
        <td align="center">이희영</td>
        <td align="center">강소영</td>
        <td align="center">김종원</td>
        <td align="center">박상훈</td>
        <td align="center">이한솔</td>
    </tr>
    <tr>
        <td><img src="https://github.com/HeeYeong91/project_shoppingmall_call/assets/139057065/960c0e7e-ad28-4f1d-82d0-b4b7be4d3a5c" height=150 width=150></td>
        <td><img src="https://github.com/HeeYeong91/project_shoppingmall_call/assets/139057065/9e7da88f-0f0e-43e9-a302-aa15c5782a0a" height=150 width=150></td>
        <td><img src="https://github.com/HeeYeong91/project_shoppingmall_call/assets/139057065/4bd1b60f-c42a-4799-83df-6f22c46fcc4a" height=150 width=150></td>
        <td><img src="https://github.com/HeeYeong91/project_shoppingmall_call/assets/139057065/50db4e93-aca9-482d-b889-a1239de224e0" height=150 width=150></td>
        <td><img src="https://github.com/HeeYeong91/project_shoppingmall_call/assets/139057065/4f1a8bdf-8fc0-41fe-a23b-1e8f24317f52" height=150 width=150></td>
    </tr>
    <tr>
        <td align="center"><a href="https://github.com/heeyeong91">@heeyeong</a></td>
        <td align="center"><a href="https://github.com/soyeong-elena">@soyeong</a></td>
        <td align="center"><a href="https://github.com/911kimjonga">@jongwon</a></td>
        <td align="center"><a href="https://github.com/sjm601">@sanghoon</a></td>
        <td align="center"><a href="https://github.com/lhansol1996">@hansol</a></td>
    </tr>
</table>
<br /> <br />

## :pushpin: 2. 프로젝트 기능
## 1. 메인 페이지 구현

![1 메인페이지구현](https://github.com/HeeYeong91/project_shoppingmall_call/assets/139057065/6b28a271-ebb8-4e15-bfc5-ac333b4e28c5) <br />
[목차](#page_facing_up-목차)

## 2. 회원가입 및 로그인 구현

![2 회원가입및로그인구현](https://github.com/HeeYeong91/project_shoppingmall_call/assets/139057065/85f678f5-6a79-4fe3-9770-ef6cb0aeb8d8) <br />
[목차](#page_facing_up-목차)

## 3. 제품 리스트 화면 구현

![3 제품리스트화면구현](https://github.com/HeeYeong91/project_shoppingmall_call/assets/139057065/8313220f-85c3-44b4-93fd-77541c6edc30) <br />
[목차](#page_facing_up-목차)

## 4. 제품 상세페이지 구현
* ProductDetailController.java <br />
* (1) 상세 페이지 요청(GET) <br />
* 파라미터로 상품번호를 받아 해당 상품 정보 출력 <br />
* 해당 상품에 평점 출력, 추천 상품 출력 <br />
* (2) 제품 수량 변경 요청(POST) <br />
* 장바구니 담기 욫ㅇ 시 해당 제품이 장바구니에 없으면 장바구니에 상품 추가 <br />
* 이미 장바구니에 해당 상품이 존재 시 기존 수량에 선택한 수량만큼 수량 추가 <br />

![4 제품상세페이지구현](https://github.com/HeeYeong91/project_shoppingmall_call/assets/139057065/c303bb26-1837-46fa-9e78-757f9a24abdb) <br />
[목차](#page_facing_up-목차)

## 5. 리뷰 구현

![5 리뷰목록](https://github.com/HeeYeong91/project_shoppingmall_call/assets/139057065/49f0c58b-ad2e-4410-afd8-3d8f94117875) <br />
![5 리뷰작성](https://github.com/HeeYeong91/project_shoppingmall_call/assets/139057065/28ac82cf-cdfe-4885-864e-abc3fba220c3) <br />
[목차](#page_facing_up-목차)

## 6. 매장 위치 카카오지도 API구현

![6 매장위치](https://github.com/HeeYeong91/project_shoppingmall_call/assets/139057065/d91d5381-6169-4497-9fb7-978cdf4e4fd4) <br />
[목차](#page_facing_up-목차)

## 7. 장바구니 구현
* CartController.java <br />
* (1)장바구니 화면 요청(GET) <br />
* 장바구니 목록, 총금액 출력 <br />
* (2)장바구니 삭제 & 수량변경 요청(GET) <br />
* 장바구니에서 상품 삭제 <br />
* 수량 변경 시 수량은 1보다 작을 수 없고 9보다 커질 수 없다고 가정해서 적용 <br />
* (3)주문하기 요청(POST) <br />
* 주문하기 요청 <br />
* 결제 API를 사용하지 않아 주문하기 요청했을 때 결제까지 됐다고 가정하고 구현 <br />

![7 장바구니구현](https://github.com/HeeYeong91/project_shoppingmall_call/assets/139057065/10335ff6-1a9f-405c-86e6-43e6409ca68e) <br />
[목차](#page_facing_up-목차)

## 8. 주문 구현

![8 주문구현](https://github.com/HeeYeong91/project_shoppingmall_call/assets/139057065/b5e1fb3b-e35f-4502-a825-9599ff29aba4) <br />
[목차](#page_facing_up-목차)
