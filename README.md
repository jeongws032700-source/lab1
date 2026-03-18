# Maria database 설치 및 SQL 연습

`실습 (1)` 폴더의 3번 과제를 정리한 저장소입니다.

Node.js, Express, MariaDB를 사용해 자재 정보를 등록, 조회, 수정할 수 있는 자재 관리 웹 애플리케이션을 구현했습니다.

## 주요 기능

- 자재 목록 조회
- 자재 상세 조회
- 자재 등록
- 자재 수정
- 상태, 수량, 단가, 입고일 등 자재 정보 관리

## 폴더 구성

```text
content/
  server.js
  package.json
  static/
  templates/
```

- `server.js`: Express 서버와 MariaDB 연동 코드
- `static/`: CSS, 이미지 등 정적 파일
- `templates/`: 목록, 상세, 등록, 수정 화면 템플릿

## 실행 방법

```bash
apt update -y
```

기본 실행 포트는 `3000`입니다.

## 데이터베이스 설정

`content/server.js` 기준 연결 정보는 아래와 같습니다.

- host: `localhost`
- user: `testuser`
- password: `1234`
- database: `testdb`

MariaDB에 `material` 테이블이 준비되어 있어야 정상 동작합니다.
