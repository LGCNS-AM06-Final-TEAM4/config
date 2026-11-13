# 리테일 도메인 최종 프로젝트 config

backend의 Config Server가 읽는 설정 파일 저장소입니다. 서비스 코드는 [backend](https://github.com/LGCNS-AM06-Final-TEAM4/backend) 레포에 있습니다.

## 파일 규칙

파일 이름은 `서비스이름-프로필.yml`로 씁니다. 예를 들어 `gateway-service.yml`은 모든 프로필에 공통으로 쓰이고, `gateway-service-dev.yml`은 dev 프로필에서만 쓰입니다. 서비스가 정해지면 파일을 추가합니다.

DB 비밀번호나 JWT 키 같은 값은 평문으로 올리지 않습니다. Config Server 암호화로 `{cipher}` 값을 만들어 넣거나 환경 변수로 넘깁니다.

## 브랜치

Config Server가 `main`을 읽기 때문에 이 레포는 `main` 하나만 씁니다. 설정을 바꿀 때도 이슈 번호로 브랜치를 만들어 PR로 합칩니다. 나머지 규칙은 backend 레포의 [협업규칙.md](https://github.com/LGCNS-AM06-Final-TEAM4/backend/blob/develop/docs/협업규칙.md)를 따릅니다.
