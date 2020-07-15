# Docker 명령어

### 버전 확인
`
docker -v
`

### docker 이미지 가져오기
`
docker pull [이미지 이름]:[태그]
`

### 이미지 확인하기
`
docker images
`

### 컨태이너 생성하기
`
docker create [옵션][이미지 이름]:[태그]

example)

docker create -i -t centos:7
`
* -i: 상호 입출력
* -t: tty를 활성화하여 bash 쉘을 사용

### 컨태이너 실행하기
`
docker start centos:7
`

### 컨태이너 들어가기
`
docker attach centos:7
`

### 컨태이너 만들고 실행하기
`
docker run [옵션] [이미지 이름]:[태그]
`
* -i: 상호 입출력
* -t: tty를 활성화하여 bash 쉘을 사용

### 컨태이너 목록 확인
`
docker ps [옵션]
`
* -a: 정지된 컨태이너까지 확인

### 컨태이너 이름 변경
`
docker rename [기존 이름] [변경하고자 하는 이름]
`

### 컨태이너 삭제
`
docker rm [옵션] [컨태이너 이름]
`
* -f: 강제로 실행

### 컨테이너 정지
`
docker stop [컨태이너 ID or 이름]
`

### 컨태이너 실행하고 외부에 노출
`
docker run -i -t -d --name mywebserver -p 80:80 ubuntu:14.04
`
* 80:80은 [외부에서 사용할 포트][컨태이너 내부의 포트]
* -d: Background에서 실행
* -i: 상호 입출력
* -t: tty를 활성화하여 bash 쉘을 사용
