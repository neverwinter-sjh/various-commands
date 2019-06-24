# linux-commands
리눅스 자주 쓰는 명령어 모음

### sh 파일 실행권한
```
chmod +x finename.sh
```

### 현재 활성화된 포트 목록
* To format it in a nice, readable way; use :
```
sudo lsof -i -n -P | more
```
* To view view only TCP connections :
```
sudo lsof -i -n -P | grep TCP | more
```
* To view view only UDP connections :
```
sudo lsof -i -n -P | grep UDP | more
```
