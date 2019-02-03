# server-monitoring

## TPS, PPS, HPS, RPS

### TPS \(Transaction Per Second\)

클라이언트 서버 환경에서 비롯된 단어. 클라이언트/서버 환경에서 어플리케이션이 직접 서버 \(데이터베이스\)에 접속하여 쿼리, 트랜젝션을 요청했기 떄문에, 서버\(데이터베이스\)의 성능을 측정하는 기준으로 초당 몇건의 트랜잭션을 수행했느냐에 대한 성능 지표

### PPS \(Page Per Second\)

특정 URL을 호출했을 떄, 서버작업의 수행 결과를 화면에 출력하기 위해 CSS, Image 파일과 같은 정적\(static\) 컨텐츠를 다운로드 받는 성능 측정 기준

### HPS \(Hit Per Second, RPS: Request Per Second\)

정적인 컨텐츠를 제외한 동적 컨텐츠 \(XML, JSON 등\) 요청에 대한 응답시간을 측정하는 기준

## TPS vs 평균 응답 시간

### 단위시간당 처리건수

단위시간당 최대 처리건수를 의미하는 TPS를 사용하는것이 적합

