<h1>project_bus_station_navigation</h1>
<p>GPS 기반 가장 가까운 버스 정류장 정보와 버스 도착시간 표시하는 소형 단말기 제작</p>

<h2>동작 흐름</h2>
<pre>
1. GPS 모듈로 사용자 현재 위치 수신
2. 공공데이터 API에서 근처 정류장 조회(위치 기반)
3. 해당 정류장의 도착 예정 버스 정보 받아옴.
    도착 예정 버스 정보는 전국 버스 정보 API 활용(정류소 조회 및 도착 예정 정보)
    https://www.data.go.kr/
4. 정보 출력
    OLED 이용하여 화면에 도착시간 빠른 순으로 버스 정류장 이름과 버스 번호, 남은 시간, 
    사용자의 현재 위치에서 버스정류장까지 도보 시간 출력
5. 1분마다 주기적으로 갱신
</pre>


<h2>기술 스택</h2>

<pre>
1. 위치 기반 처리
2. API 통신
3. 텍스트 디스플레이로 데잍 출력
4. 시리얼 통신(UART)
5. 전원 공급(배터리나 보조배터리 이용)
</pre>

<h2>필요 준비물</h2>
<pre>
Raspberry Pi
NEO-6M(https://www.devicemart.co.kr/goods/view?no=1321968&srsltid=AfmBOorrvlQRPtdi3rQ5yU_xW2kwgXNpaGIRC5D_vi3mrPR91V55Ifnk)
OLED(https://smartstore.naver.com/toolboxkorea/products/10337644136?NaPm=ct%3Dmauv6xn6%7Cci%3DER10b7ab94%2D3491%2D11f0%2Dafb4%2Deeae0d0a113e%7Ctr%3Dpla%7Chk%3D072755d2631f86991ddd5b4ee5e4e7c22b61a16c%7Cnacn%3DsIn5Bgw2Omq2)
python programming
보조배터리
</pre>
