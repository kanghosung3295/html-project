@ -0,0 +1,117 @@
<!DOCTYPE html>
<html lang="ko">  
<!-- 문서 타입 선언, 한국어로 설정 -->
<head>
  <meta charset="UTF-8">
  <!-- 문자 인코딩은 UTF-8 -->
  <title>Produce 정치인</title>
  <style>
    /* css 디자인 */
    body {
      font-family: 'Arial', sans-serif;
      background-color: #fefbee;
      display: flex;
      flex-direction: column;
      /* flex사용해서 모든 요소 세로 방향 중앙 정렬 */
      align-items: center;
      padding: 40px;
    }
/* 전체 페이지 중앙 정렬, 수직 정렬 구조 */
    h1 {
      font-size: 40px;
      margin-bottom: 50px;
    }

    .search-box{
        margin-bottom: 30px;
    }
/* 검색창 스타일 지정 */
    input[type="text"]{
        padding: 8px 12px;
        font-size: 14px;
        width: 200px;
        border: 1px solid #aaa;
        border-radius: 6px;
    }

    .grid {
      display: grid;      
      grid-template-columns: repeat(3, 100px);
      grid-gap: 70px;
    }
/* 카드를 3개씩 정렬하는 격자 레이아웃 */
    .card {
      width: 150px;
      height: 150px;
      border: 2px solid black;
      border-radius: 10px;
      background-color: white;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      /* 클릭할 수 있는 모양(손 모양으로 마우스 커서 바뀜) */
      cursor: pointer;
    }

/* 카드 하나의 형태 : 네모 테두리와 내부 요소 세로 정렬 */
    .card img{
        width: 100px;
        height: 100px;
        /* 카드 안의 이미지 크기 맞게 해서 안잘리게 함 */
        object-fit: cover; 
        border-radius: 8px;
    }
  </style>
</head>
<body>

  <h1>Produce 정치인</h1>

<div class="search-box">
    <input type="text" id="searchInput" placeholder="정치인 검색">
    <!-- 검색창 input placeholder는 입력 전 안내해주는 텍스트-->
</div>
<div class="grid" id="cardGrid">
    <div class="card">
    <img src = "c:\Users\user\OneDrive\바탕 화면\새 폴더\강호성35.jpg">
    <span>강호성</span>
</div>
    <div class="card">
    <img src = "https://newsimg.sedaily.com/2021/12/09/22V868A64C_3.jpg">
    <span>이 재 명</span>
    </div>
    <div class="card">
    <img src = "https://image.edaily.co.kr/images/photo/files/NP/S/2023/03/PS23031700860.jpg">
    <span>윤 석 열</span>
    </div>
    <div class="card">
    <img src = "https://cdn.hankooki.com/news/photo/202411/211997_294341_1732954110.jpg">
    <span>winter</span>
    </div>
    <div class="card">
    <img src = "https://pimg.mk.co.kr/news/cms/202504/07/news-p.v1.20250407.de7f48cc1fd24ad197bcba670d5e6449_P1.jpg">
     <span>이 름</span>
    </div>
    <div class="card">
    <img src = "https://thumbnews.nateimg.co.kr/view610///news.nateimg.co.kr/orgImg/jn/2024/02/18/10bc0d844039f8.jpg">
    <span>이 름</span>
    </div>
    <div class="card">
    <img src = "https://img2.sbs.co.kr/img/seditor/VD/2023/05/24/fB51684893425345-640-0.jpg">
    <span>이 름</span>
    </div>
    <div class="card">
    <img src = "https://newsimg.sedaily.com/2023/12/15/29YISQE7IR_1.jpg">
    <span>이 름</span>
    </div>
    <div class="card">
    <img src = "https://image.ytn.co.kr/general/jpg/2023/0809/202308090915012150_d.jpg">
    <span>이 름</span>
    </div>
  </div>
  <!-- 각 카드에 이미지랑 텍스트 넣을 수 있음 -->
<!-- 추후 스크롤 아니면 페이지네이션 기능 추가 예정 -->

</body>
</html>
