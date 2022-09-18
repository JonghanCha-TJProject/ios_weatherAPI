# Guidelines



# 요구사항


- 지역별 날씨를 보여주는 어플리케이션을 구현합니다.
- 지역 이름에 **"se"** 가 포함된 지역을 대상으로 오늘, 내일 날씨를 보여줍니다.
- 날씨 정보는 지역 이름, 날씨 아이콘, 날씨 요약, 현재 온도, 습도로 구성됩니다.

# API

- [https://www.metaweather.com/api/](https://www.metaweather.com/api/) – MetaWeather의 Open API를 사용해주세요.
    1. **Location Search** - /api/location/search/?query=(query)를 사용해서 검색어 **"se"** 로 검색되는 지역 목록을 반환받습니다.
    2. **Location** - /api/location/(woeid)/를 사용해서 각 지역별 날씨 정보를 반환받습니다.

        consolidated_weather 필드의 하위 필드를 사용해서 각 날씨를 구성합니다.


|field|desc|
|:--:|:--:|
|weather_state_name|날씨 요약|
|weather_state_abbr|아이콘 이미지 정보|
|the_temp|현재 날씨|
|humidity|습도|


# 개발 환경

- **언어** –  Swift

