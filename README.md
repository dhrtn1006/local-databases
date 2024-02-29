# LOCAL DB 환경 구성

## 설치

### GIT CLONE
```bash
git clone 
```

### .gitkeep 파일 삭제
```bash
find . -name .gitkeep -exec rm -f {} \;
```

## 실행

### COMPOSE 실행
```bash
docker-compose up -d
```

### DATA DUMP
```bash
mysqldump -u 사용자이름 -p 비밀번호 DB명 > dump-DB명-202301011159.sql
```

### DATA LOAD
```bash
mysql -u 사용자이름 -p DB명 < dump-DB명-202301011159.sql
```
