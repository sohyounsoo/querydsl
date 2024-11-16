## Trouble Shooting
### 원인

QHello를 임포트 할 때, src/main 쪽의 QHello를 사용하는것 같은데,

build 경로에서 직접 사용해야 되는 문제가 발생



### 해결

settings or properties -> build tools -> gradle 에서 설정한 Build and Run

Gradle에서 Intellij로 변경한 부분 Gradle로 바꾸면 build -> generated -> sources -> ... -> main -> ... -> QHello

여기서 main 폴더가 root 폴더가 되면서 import 가능한 상태로 바뀜
