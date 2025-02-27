# HTTP 기본

## HTTP

HTTP : Hyper Text Transfer Protocol

<span style="color:#808080">HTML, Text, Image, 음성, 영상, 파일, Json … 등 모든걸 HTTP를 사용해서 전송</span>

## 클라이언트 서버 구조

Request Response 구조

클라이언트는 서버에 요청을 보내고, 응답 대기

서버는 요청에 대한 결과를 만들어서 응답

## Stateful Stateless

- Stateful : 상태유지 (점원이 바뀌면 곤란)

- Stateless : 무상태 (점원이 바뀌어도 영향X)

## 비연결성

- HTTP는 기본이 연결을 유지하지 않음

- 일반적으로 초 단위의 이하의 빠른 속도로 응답

- 1시간 동안 수천명이 서비스를 사용해도 실제 서버에서 동시에 처리하는 요청은 매우 작음

- 서버 자원을 매우 효율적으로 사용할 수 있음

## 비연결성의 한계

- TCP/IP 연결을 새로 맺어야 함

- 3 way handshake 시간 추가

- 웹 브라우저로 사이트를 요청하면 수 많은 자원이 함께 다운로드

지금은 HTTP 지속 연결(Persistent Connections)로 문제 해결

## HTTP메시지

구조 - 시작라인 / 헤더 / 공백 / 바디

시작라인 : 메서드 & 요청대상 & 버전 & 응답메시지

헤더 : 부가정보 (바디 내용, 크기, 압축, 인증 … )

바디 : 실제 전송할 데이터
