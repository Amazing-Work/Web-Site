<!doctype html>
<html lang="ko">

<head>
  <meta charset="utf-8">
  <style>
    .more {
      display: block;
      width: 55px;
      height: 16px;
      background-image: url('https://s.pstatic.net/static/www/img/2017/sp_nav_v170523.png');
      background-position: 0 -78px;
    }

    .blind {
      position: absolute;
      overflow: hidden;
      clip: rect(0 0 0 0);
      margin: -1px;
      width: 1px;
      height: 1px;
    }

    .more:hover,
    .close:hover {
      cursor: pointer;
    }

    .close {
      display: block;
      background-image: url('https://s.pstatic.net/static/www/img/2017/sp_nav_v170523.png');
      width: 42px;
      height: 16px;
      background-position: -166px -78px;
    }

    .board {
      font-family: '돋움';
      font-size: 13px;
      position: absolute;
      top: 30px;
      width: 410px;
      height: 135px;
      background: pink;
    }

    .list {
      float: left;
    }

    .list li {
      list-style: none;
      margin-top: 5px;
    }

    .list li:hover {
      text-decoration: underline;
      cursor: pointer;
    }
  </style>
  <script src="http://code.jquery.com/jquery-1.8.2.min.js"></script>
  <script>
    $(document).ready(function () {
      $('.board').hide();
      $('.more').click(function () {
        $('.more').toggleClass('close');
        $('.board').toggle();
      });
    });
  </script>

</head>

<body>
  <span class="more">
    <span class="blind">더보기 V</span>
  </span>
  <div class="board">
    <ul class="list">
      <li>가계부</li>
      <li>날씨</li>
      <li>네이버 예약</li>
      <li>네이버 캐스트</li>
      <li>네이버 클라우드</li>
    </ul>
    <ul class="list">
      <li>만화 / 웹툰</li>
      <li>매거진캐스트</li>
      <li>메모</li>
      <li>뮤직</li>
      <li>부동산</li>
    </ul>
    <ul class="list">
      <li>영화</li>
      <li>오디오클립</li>
      <li>오피스</li>
      <li>웹소설</li>
      <li>자동차</li>
    </ul>
  </div>
</body>

</html>
