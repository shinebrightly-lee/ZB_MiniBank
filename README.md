# ZB_MiniBank
![header](https://capsule-render.vercel.app/api?type=waving&color=gradient&height=300&section=header&text=MiniBank&desc=first_mini_project&fontSize=90)


간단한 기본 계좌시스템을 목적으로 하는 프로젝트 입니다.

<br>

---
<br>

## ⏳ 프로젝트 기간 ⌛ <br>
　23.07.18 ~ 

<br>
<br>

---
<br>

## 📋 프로젝트 주요 기능　( 기능 클릭시 상세 기능 설명보기 가능 ) <br>
<br>

📢 공통 조건 사항 <br>
　　- 사용자는 사용자의 게좌에만 접근이 가능하며 타인의 계좌에 접근 불가능 하다. <br>
　　- 사용자의 계좌에 가지고 있을 수 있는 금액은 최대 20억으로 제한되어 있다. <br>
　　- 사용자가 한번에 거래할 수 있는 최대 금액은 5000만원으로 제한되어 있다. <br>
　　- MiniBank 끼리만 거래가 가능하다. ( 타은행 거래 불가 ) <br>
<br>

<details>
<summary> 회원가입 기능 🖱 </summary>
  <br>
사용자는 회원가입을 할 수 있다. <br>
일반적으로 모든 사용자는 회원가입시 USER 권한 (일반 권한) 을 지닌다. <br>
회원가입시 아이디와 패스워드를 입력받으며, 아이디는 unique 해야한다. <br><br>
　+ 입력 : id, pw
<br><br>
</details>

<details>
<summary> 로그인 기능 🖱 </summary>
  <br>
사용자는 로그인을 할 수 있다. <br>
로그인시 회원가입때 사용한 아이디와 패스워드가 일치해야한다.  <br><br>
　+ 입력 : id, pw 
  <br><br>
</details>

<details>
<summary> 계좌 생성 기능 🖱  </summary>
  <br>
사용자는 계좌를 생성할 수 있다. <br>
단 최대 10개까지 가능하다. <br><br>
　+ 출력 : 현재 생성된 계좌
  <br><br>
</details>

<details>
<summary> 계좌 조회 기능 🖱  </summary>
  <br>
사용자는 개설된 계좌의 목록을 조회할 수 있다. <br><br>
　+ 출력 : 생성했던 계좌들의 목록
  <br><br>
</details>

<details>
<summary> 계좌 삭제 기능 🖱  </summary>
  <br>
사용자는 계좌를 선택하여 삭제할 수 있다. <br>
삭제시 한번 더 비밀번호를 입력 받는다. <br>
삭제 시 선택한 계좌의 금액은 0원이여야 가능하며, 복구는 불가능 하다. <br><br>
　+ 입력 : 선택한 계좌, pw <br>
　+ 출력 : 계좌에 금액이 남아 있다면 남은금액과 함께 error 문구 출력 <br>
　　　　　　정상 삭제가 되었다면 계좌 성공 문구 출력
  <br><br>
</details>

<details>
<summary> 계좌 입금 기능 🖱  </summary>
  <br>
사용자는 본인의 계좌에 입금이 가능하다. <br>
입금시 금액에 제한은 없으며 입금 금액을 입력 받는다. <br>
간단한 메모를할 수 있다. (선택) <br><br>
　+ 입력 : 입금 금액, 메모 <br>
　+ 출력 : 입금 후 잔액
  <br><br>
</details>

<details>
<summary> 계좌 송금 기능 🖱  </summary>
  <br>
사용자는 타인에게 송금이 가능하다. <br>
( 그러나 같은 은행끼리만 송금이 가능하다. / MiniBank 내에서만 서로 가능 ) <br>
송금시 한번더 비밀번호를 입력 받는다. <br>
간단한 메모를할 수 있다. (선택) <br>
송금시 계좌번호와, 계좌명, 금액을 입력 받으며, <br>
계좌번호 및 계좌명이 불일치 할 경우 송금은 실패한다. <br>
계좌의 잔액보다 송금하는 금액이 높을 경우에도 송금은 실패한다. <br>
송금 금액이 0원 이하일 경우에도 송금은 실패한다. <br><br>
　+ 입력 : 계좌번호, 계좌명, 송금 할 금액, pw, 메모 <br>
　+ 출력 : 정상 송금 시 성공 문구 출력 <br>
　　　　　 잔액이 맞지 않을 경우 error 문구 출력 <br>
　　　　　 계좌번호 및 계좌명이 맞지 않을 경우 error 문구 출력
  <br><br>
</details>

<details>
<summary> 계좌 인출 가능 🖱  </summary>
  <br>
사용자는 계좌의 금액을 인출할 수 있다. <br>
인출시 한번 더 비밀번호를 입력 받는다. <br>
계좌의 금액보다 인출할 금액이 더 높을 경우 계좌의 잔액은 인출할 수 없다. <br>
0보다 낮은 금액도 인출할 수 없다. <br><br>
　+ 입력 : 인출 금액, pw <br>
　+ 출력 : 인출 성공시 성공 문구 출력 <br>
　　　　　 인출 금액이 맞지 않을 경우 error 문구 출력 
  <br><br>
</details>

<details>
<summary> 계좌 송금 이력 조회 기능 🖱  </summary>
  <br>
사용자는 송금한 이력을 조회 할 수 있다. <br>
아무조건이 없는경우 -> 현재 ~ 한달간 송금 이력을 보여준다. <br>
조건 선택은 계좌를 생성한 날부터 현재까지 날짜를 선택 할 수 있다. <br>
( 최근 ~ 오래된 순으로 20 개씩 출력 가능하며, 더보기를 선택 할 경우 오래된 경과를 추가로 가져온다. ) <br><br>
　+ 입력 : 원하는 날짜, 더보기 ( 날짜 및 더보기는 선택사항이므로 입력 받지 않은채로도 진행 가능하다. ) <br>
　+ 출력 : 기간, 송금이력을 묶어서 출력 ( 송금 보낸이, 송금 받은이, 송금액, 보내고 난 뒤 잔액, 날짜&시간 ) <br>
  <br><br>
</details>
  
<br>
<br>

---
<br>

## 🗺 ERD 

<br>

![image](https://github.com/shinebrightly-lee/ZB_MiniBank/assets/128344191/38d3b643-1c2f-4170-9b4c-d13ff6e999d6)


<br>
<br>

---
<br>
<div align=center><h1>📚 Stacks</h1></div>

<div align=center> 
  <img src="https://img.shields.io/badge/java-007396?style=for-the-badge&logo=java&logoColor=white">
  <img src="https://img.shields.io/badge/spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white">
  <img src="https://img.shields.io/badge/gradle-02303A?style=for-the-badge&logo=gradle&logoColor=white">
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=MySQL&logoColor=white"/>
</div>



