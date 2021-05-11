# Klush Team Project🚀
이번에 진행 했던 klsuh team project는 순수 개발시간의 비중을 높이기 위해<br/>
이미 서비스 중인 사이트의 기획이나 디자인을 참고하여<br/>
진행하는 프로젝트입니다.

대상 사이트는 코리아 LUSH 사이트로, 초기세팅 부터 전부 직접 구현했으며 Front와 연결하여<br/>
보편적인 쇼핑몰의 기본 기능을 구현, 사용자가 실제 사용할 수 있을 정도의 서비스를 개발했습니다.

## 참여 인원과 기간
2021.03.15 ~ 2021.03.26<br/>
백엔드 총 3명, 프론트 총 3명의 인원으로 진행

## 기술 스택
Back-End : `Python`, `Django web framework`, `Bcrypt`, `JWT`, `My SQL`<br/>
Common : `AWS(EC2,RDS)`, `RESTful API`

## 구현한 기능
### 공통 사항
- ERD Modeling

### USER ENDPONIT
- 회원가입
- 로그인

### PRODUCT ENDPOINT
- 상품 리스트
- 상품 디테일
- 상품 조건별 필터 리스트 << REQUEST 에서 쿼리 파라미터를 받아서 필요한 기준으로 상품 리스트를 필터링해서 보여준다.
예를들어, 신상품은 'is_new'라는 파라미터가 들어온다면, 장고의 쿼리셋에서 해당 필터기준을 objects.filter(key=key) 로 가져와서 가공한후 클라이언트 쪽에 데이터를 제공한다.
 
### ORDER ENDPOINT
- 장바구니 생성
- 장바구니 제품 추가

### Database
- CSV 파일 제작 후 API를 구성하여 데이터 등록

### 배포
- AWS Ec2와 RDS를 통하여 서버 배포 <<

---

## 추후 리팩토링 예정
#### USER ENDPOINT
- 회원 마이페이지 구축 (회원 정보, 게시판, 배송지 관리)

#### ORDER ENDPOINT
- 장바구니 수정, 삭제
- 주문하기

#### PRODUCT ENDPOINT
- 상품별 리뷰 등록

<br/><br/>
