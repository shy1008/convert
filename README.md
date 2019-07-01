# 단위변환 클래스
순수한 PHP로 제작된 단위 변환 라이브러리 입니다.

## 설치
지니 단위변환기는 컴포저를 이용하여 배포/설치 됩니다.

```
composer require jiny/convert
```

## 사용방법
신규 파일을 생성후, 컴포저 오토로드 코드를 삽입합니다.
단위 변환에 대한 객체를 생성합니다.

### 셈플코드
```php
<?php
// 오토로드
require "../../../autoload.php";

// 객체생성 
$inch = new Jiny\Convert\Length\Inch(1);
echo $inch->centi();
```

### 단위값 설정
변환값의 설정은 2가지 방식으로 제공을 합니다.
먼저, 변환되는 단위 값을 객체 생성 인자값으로 전달 합니다.  
또는 객체 생성후에 `setter 메소드`를 통하여 객체의 변환값을 변경할 수 있습니다.

```php
$inch->setValue(100);
```

### 변환값 확인
단위 객체에 설정된 기본값을 이용하여, 변환된 값을 출력할 수 있습니다.
변환 하고자 하는 메소드를 호출합니다.

```php
// 설정된 인치(inch) 값을 센치미터로 변환 합니다.
echo $inch->centi();
```

## [길이](length.md)
단위 길이를 변경할 수 있습니다.
- 미터
- 센치
- 밀리미터
- 킬로미터
- 인치
- 피트
- 야드
- 마일
- 자
- 간
- 정
- 리
- 해리

## 넓이
- 제곱미터
- 야르
- 헥타르
- 제곱킬로미터
- 제곱피트
- 제곱야드
- 에이커
- 평방자
- 평
- 단보
- 정보

## 무게
- 밀리그램
- 그램
- 킬로그램
- 톤
- 킬로톤
- 그래인
- 온스
- 파운드
- 돈
- 냥
- 근
- 환

## 부피
- 시시
- 밀리리터
- 데시리터
- 리터
- 세제곱 센치미터
- 세제곱 미터
- 세제곱 인치
- 세제곱 피트
- 세제곱 야드
- 갤런
- 배럴
- 온스
- 홈
- 되
- 말

## 온도
- 섭씨
- 화씨
- 절대
- R

## 압력
- 기압
- 파스칼
- 헥토 파스칼
- 킬로 파스칼
- 메가 파스칼
- dyne
- 밀리바
- 바
- kfg/cm^2
- 파사이
- 수은주 밀리미터
- inchHg
- 수주밀리미터
- inchH2O

## 속도
- m/s
- m/h
- km/s
- km/h
- in/s
- in/h
- ft/s
- ft/h
- mi/s
- mi/h
- 노트(kn)
- 마하(mach)

## 연비
- km/l
- mi/g
- l/100km

## 데이터
- 비트
- 바이트
- 킬로 바이트
- 메가 바이트
- 기가 바이트
- 테라 바이트
- 페타 바이트
- 엑사 바이트

## 시간
