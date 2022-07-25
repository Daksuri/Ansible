# Ansible

## Ansible 이란?
인프라 관리를 코드 기반으로 자동화하는 도구!
IaC를 지향하는 오픈소스 기반의 자동화 관리 도구!!

[동작] 
자동 구촉/관리 하려는 원격 인프라에 명령을 전달하는 방식으로 동작

## Ansible이 갖는 특징

### 1) Agentless

Ansible의 경우는 SSH를 기반으로 원격 서버에 명령을 전달하기 때문에 Agent가 불필요합니다.

※ Agent가 필요 없다는 건, 각 원격 서버에 접속해서 Agent를 설치해줄 필요가 없다는 것!! ※

※ Agent 설치 단계를 제거하여 인프라 구축을 더 자동화에 가깝게 만든 것!! ※

### 2) 접근 용이성

Ansible은 이러한 명령 모음집(뒤에서 소개할 playbook)을 YAML형식의 파일로 관리 합니다.
YAML 파일의 훌륭한 가독성 덕분에 사용자들이 느끼는 앤서블의 진입장벽이 낮습니다.

### 3) 멱등성

멱등성이란 여러번 수행해도 같은 결과를 뱉는 성질을 말합니다.

앤서블은 YAML로 관리되는 명령집을 여러번 수행하더라도 언제나 같은 결과가 나올 수 있도록 여러가지 관리를 합니다.


## Ansible 설치

Ansible은 Python의 pip, OS의 패키지 관리도구를 이용하여 설치 가능

Ansible을 이용하여 Ansible 버전을 설정하고 설치하는것을 추천!!
Ansible은 2.x, 3.x, 4.x 각 버전에 따라 문법이 다르기 때문에 테스트 환경과 실행환경의 버전을 고정하여 실행하는 것이 좋습니다.


### Python 
```
$ pip install ansible

# 설치 할 Ansible 버전을 설정
$ pip install ansible==[version]
```

### Ubuntu
```
$ apt install ansible
```
