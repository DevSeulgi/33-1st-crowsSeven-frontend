## 크로우즈세븐

이 프로젝트는 [크로우캐년](https://crowcanyon.co.kr/) 사이트를 참조하여 학습목적으로 진행되었습니다. </br>
</br>
![crwosSeven_main](https://user-images.githubusercontent.com/97112697/172040440-b586430d-e7ea-445e-9c95-0d4141fa5795.gif)</br>
</br>
**전체 데모영상 :** https://youtu.be/--gfsEindSE
</br>
- _[`프론트엔드` GitHub repository](https://github.com/wecode-bootcamp-korea/33-1st-crowsSeven-frontend)_ </br>
- _[`백엔드` GitHub repository](https://github.com/wecode-bootcamp-korea/33-1st-crowsSeven-backend)_
</br>

## 기술 스택
- `프론트엔드`: JavsScript, ReactJS, React-Router, HTML5, SASS
- `백엔드`: Python, Django, AWS
- `협업Tool`: Git, Slack, Trello, Notion
</br>

## 개발 기간 및 인원
**개발 기간 :** 5월 23일 - 6월 3일 (11일)
</br>

### 프론트엔드
<table>
  <tr>
    <td align="center">
      <a href="https://github.com/DevSeulgi"
        ><img
          src="https://avatars.githubusercontent.com/u/97112697?v=4"
          width="100px;"
          alt=""
        /><br /><sub><b>박슬기</b></sub></a
      ><br />
    </td>
    <td align="center">
      <a href="https://github.com/kimwanyoung"
        ><img
          src="https://avatars.githubusercontent.com/u/78637786?v=4"
          width="100px;"
          alt=""
        /><br /><sub><b>김완영</b></sub></a
      ><br />
    </td>
    <td align="center">
      <a href="https://github.com/yoohaaeun"
        ><img
          src="https://avatars.githubusercontent.com/u/101792909?v=4"
          width="100px;"
          alt=""
        /><br /><sub><b>유하은</b></sub></a
      ><br />
    </td>
    <td align="center">
      <a href="https://github.com/Yumjong"
        ><img
          src="https://avatars.githubusercontent.com/u/96937488?v=4"
          width="100px;"
          alt=""
        /><br /><sub><b>염종은</b></sub></a
      ><br />
    </td>
    <td align="center">
      <a href="https://github.com/sourmix"
        ><img
          src="https://avatars.githubusercontent.com/u/75124027?v=4[ㅠㅠㅠ"
          width="100px;"
          alt=""
        /><br /><sub><b>신윤지</b></sub></a
      ><br />
    </td>
  </tr>
</table>

### 백엔드
<table>
  <tr>
    <td align="center">
      <a href="https://github.com/onlining"
        ><img
          src="https://avatars.githubusercontent.com/u/96784345?v=4"
          width="100px;"
          alt=""
        /><br /><sub><b>김민정</b></sub></a
      ><br />
    </td>
    <td align="center">
      <a href="https://github.com/ysang989"
        ><img
          src="https://avatars.githubusercontent.com/u/67964576?v=4"
          width="100px;"
          alt=""
        /><br /><sub><b>박상연</b></sub></a
      ><br />
    </td>
  </tr>
</table>
</br>

## 구현 기능
| 이름       | 기능                               |
| --------- | --------------------------------- |
| **박슬기** | 상품 목록 페이지, 상품 상세 페이지        |
| **김완영** | 메인 페이지, Search, Nav, Footer     |
| **유하은** | 장바구니 페이지, 주문 완료 페이지         |
| **염종은** | 주문 조회 페이지, 로그인 & 회원가입 페이지  |
| **신윤지** | 리뷰 게시판 페이지, 리뷰 작성 페이지       |
</br>

## 박슬기's work
### 📖 상품 목록 페이지
![crwosSeven_product_filter](https://user-images.githubusercontent.com/97112697/172040512-da1505b8-eceb-4843-acce-5336e3a7d636.gif)</br>
</br>
**1. 상품 목록 반응형 구현**
- 4열 고정 노출을 위해 flex wrap 사용
- 각 item은 width를 %로 구현

**2. array.map을 이용하여 백엔드와 DB 연동**
- 상품명, 가격, 태그 정보 연동
- 목록의 length를 가져와 상품 갯수 표기

**3. 상품 썸네일 및 전체 버튼의 hover 구현**
- 상품 썸네일 img에 hover 시 버튼 transition

**4. 상품 목록 2열 / 4열 보기 추가**
- listType을 추가하여 false를 기본 type으로 지정, true는 2열 보기 / false는 4열보기로 구현
- true/false에 따라 해당 scss 클래스명 지정

**5. 상품 품절 상태 일 경우 태그 노출**
- Data의 state 상태에 따라 상품 Tag 노출

</br>

### 🛒 Quick Shop Modal
- 테이블을 활용하여 상품 description 레이아웃 구현
</br>

### 💡 상품 상세 페이지
![crowsSeven_productDetail](https://user-images.githubusercontent.com/97112697/172053747-b1fd3b0c-c4a0-47d4-a115-618e467ea861.gif)</br>
</br>

**1. 레이아웃 구성**
- width를 각각 60% : 40%로 주어 어느정도의 반응형에 대응할 수 있도록 구현
- 상세페이지 이미지에는 min-width 부여

**3. 상품 수량 선택**
- 1개 이하로 수량 선택 시 alert 구현 ("주문 수량은 1 이상이어야 합니다.")
- 초기값 1로 지정 up, down 버튼을 통해 수량 조절
- 선택 수량에 따른 total 가격 및 수량 변화 구현

**4. hover & transition**
- 구매하기 / 장바구니 버튼 hover 시 색상 변경 및 transition
- wish list / 상품후기 / 상품문의 / size 버튼 hover 시 색상 변경

**5. Drawer 구현**
- 상품후기 / 상품문의 버튼 클릭 시 handle~Drawer 실행으로 각 Drawer state를 반대로 전환
- Drawer Background 클릭 시 handle~Drawer 실행으로 Drawer 닫기 구현
</br>


## **Reference**
- 실무수준의 프로젝트이지만 학습용으로 만들었기 때문에 이 코드를 활용하여 이득을 취하거나 무단 배포할 경우 법적으로 문제될 수 있습니다.
- 이 프로젝트에서 사용하고 있는 사진은 [unsplash](https://unsplash.com/)에서 제공되는 무료 사진입니다.
</br>

