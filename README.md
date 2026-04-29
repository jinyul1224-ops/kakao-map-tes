<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8">
    <title>카카오맵 테스트</title>
    <!-- 카카오맵 API 불러오기 (발급받은 JavaScript 키를 입력하세요) -->
    <script type="text/javascript" src="//dapi.kakao.com/v2/maps/sdk.js?appkey=7fb46338e5f1e9dc46574762a5345faf"></script>
</head>
<body>
    <h1>내 첫 번째 카카오맵</h1>
    <!-- 지도를 표시할 영역 -->
    <div id="map" style="width:100%;height:500px;"></div>

    <script>
        var container = document.getElementById('map'); // 지도를 담을 영역의 DOM 레퍼런스
        var options = { // 지도를 생성할 때 필요한 기본 옵션
            center: new kakao.maps.LatLng(37.5665, 126.9780), // 지도의 중심좌표 (서울시청 기준)
            level: 3 // 지도의 레벨(확대, 축소 정도)
        };

        var map = new kakao.maps.LatLng(container, options); // 지도 생성 및 객체 리턴
        
        // 지도 생성 확인을 위한 콘솔 로그
        console.log("카카오맵이 로드되었습니다.");
    </script>
</body>
</html>
