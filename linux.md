# linux-commands
리눅스 자주 쓰는 명령어 모음

### sh 파일 실행권한
```
chmod +x finename.sh
```

### 현재 활성화된 포트 목록
* 모든 목록
```
sudo lsof -i -n -P | more
```
* TCP 목록만
```
sudo lsof -i -n -P | grep TCP | more
```
* UDP 
```
sudo lsof -i -n -P | grep UDP | more
```

### 서비스 중지
```
kill -9 service-id
```
