# 아이디어 정리

---

### 타켓팅 - 명품사, 고객

1. 명품사와 계약했다고 가정
2. 명품사에서 일련번호를 전부 받아옴. VS 팔린 물품에 대한 일련번호만 받아옴.(컨설팅)
3. 일련번호로 NFT 전부 발행
   3-1. 이 과정에서 모든 명품은 NFT로 등록이 된 것.
   
    3-2. 완전 무결성을 위해서 전부 다 발행
   
4. 블록체인에 기록할 것들
    - 상품의 소유자를 기록, 소유권 이전만
    - 브랜드, 제조 국가, 제조 날짜, 상품 종류, (상품명), 일련번호,
    - 소유권자가 바꼈을 때
        - 거래일자(+as기간), 소유자 지갑 주소, 판매처(구입처),

1. 소유자가 홈페이지에서 자신의 상품의 기록을 조회 가능
2. 구매 라인 : 우리 쇼핑몰 → 구매 → 구매자의 이더리움 → 명품사 이더리움 지갑
3. 중간 수수료를 떼는 것이 없으니 명품사에 우리 솔루션을 판매.
4. 환불 배송비 부담
    - 단숨 반품 : 고객 부담
    - 제품 하자 : 명품사 부담



## 기능

### 1. 필수 기능

- **로그인 / 로그아웃**
    - 기본 로그인
    - 카카오 로그인 (security, refresh token)
    

### **회원가입 / 회원 탈퇴**

- 휴대폰 문자 인증
    - [https://charlie-choi.tistory.com/225](https://charlie-choi.tistory.com/225)
- 일회성 코드 참조
    - [https://developers.google.com/identity/sms-retriever/verify#generating_a_one-time_code](https://developers.google.com/identity/sms-retriever/verify#generating_a_one-time_code)
- 서비스 인증
    - 서비스 이용 약관(필수)
    - 개인정보 수집 및 이용(필수),
    - 만 14세 이상(필수),
    - 마케팅 정보 수신 동의(선택)
- 이더리움 지갑 생성

<br>

### 마이페이지

- 개인 정보 (이름, 아이디, 비번) - 비밀번호 수정 가능, 회원탈퇴
- 관심 상품 관리(장바구니, 찜)
- 이더리움 지갑 관리(충전, 카카오페이)
    - 우리 사이트에서 이더리움을 상당량 가지고 있고 우리 사이트에서 충천
- 내가 소유한 nft 띄우기(상품 구매 내역, 일련번호 확인)

<br>

### 메인페이지

- 네브바
- 브랜드 리스트
- 상품 리스트
- 브랜드별 or 카테고리별 추천 물품(빅데이터 X), 랭킹

<br>

### 관리자

- 회원 관리
- 거래처 관리
- 상품 등록
- NFT 발행
    - 등록하는 페이지 → NFT 정보 등록 → Solidity NFT 발행



### 상품 리스트 페이지

- 필터 (상품 카테고리, 명품사 카테고리)
- 물건은 카드 또는 리스트로 출력
- 물건 이름, 가격 등
- 상품 정보는 한페이지에 제한두고 페이지 네이션



### 상품 구매 상세 페이지

- 상품 이미지, 이름 , 가격, 정보
- 구매(개수 , 장바구니, 바로 구매)
- 관심상품 추가.



## 추가 기능

- 고객사(명품사) 지갑 연동 확인? (고객의 지갑 확인이나)
  - 필요가 없는 부분이나 추후 발표 시 제대로 구현되었는지 CMD 창에서 보여주는 것 보단 홈페이지에서 보여주는 것이 낫지 않나? 라는 의견
- QnA 기록 확인(개인이 질문 남겼을 때 그거 확인하는 용도)
- 기존의 지갑에 있는 코인을 가져와서 사용할 수 있게



### 챗봇

- 카카오 챗봇으로 연결
- 위치는 모든 페이지의 최상위로 설정