# 관악구 음식점 현황
- - -
### 개요

서비스 지역의 특성에 따라 음식 배달 서비스 개발

- - -
### 분석 목표

서비스 지역의 일반음식점 데이터를 바탕으로 지리적, 사회적 특성에 알맞은 맞춤 서비스를 제공할 수 있도록 비즈니스 방향성 제시

- - -
### 데이터 확인

#### 데이터 출처

서울 데이터 열린 광장 | https://data.seoul.go.kr

다이닝코드 | https://www.diningcode.com  (웹 크롤링)

#### 데이터 정보

매장 정보(허가번호, 매장명, 주소, 업태명, 좌표 등) 및 모범음식점 정보(지정 날짜, 취소 사유 등)

- - -
### 데이터 전처리

영업상태 필터링 (22,422개 → 4,842개) → 폐업 매장 제거

KATEC 좌표 → WGS84(경위도)

- - -
### 데이터 결측치

rest_top100 에서 허가번호가 없는 매장이 확인됨 → 허가번호가 없는 매장이 더 많을 것

☞ 전체 음식점 수 결측값에 따라 매장 밀집도 또한 변화가 있을 것으로 확인됨

- - -
Redash 대시보드

http://3.26.116.20:5000/public/dashboards/WtisXUGVs2QMpF9t7R7NcI4vYpVO88nunVKztG65?org_slug=default
