# websocket-chat-server
springboot websocket-chat-server

- 빌드 파일 서버로 복사 (scp)

    ctrl+r 누르고 scp 까지 치면 이전 명령이 나오므로 빌드파일 이름 확인하고 실행.   
    scp ~/Downloads/adapter-agent-0.0.1-SNAPSHOT.war devwas:./deploy/    
    scp ~/Downloads/alert-bot-0.0.1-SNAPSHOT.war devwas:./deploy/

- 서버 접속

    ssh devwas
    비밀 번호 : shrtlqwk123!

- 배포

    cp deploy/adapter-agent-0.0.1-SNAPSHOT.war /usr/local/tomcat8/webapps/adapter-agent.war    
    cp deploy/alert-bot-0.0.1-SNAPSHOT.war /usr/local/tomcat8/webapps/alert-bot.war

## 4. 개발한 것 운영 디비 연결해 테스트 하고 싶은 경우.   

- 개발 서버에 배포한다.
- 개발 스프링 로그를 확인한다.

    tail -f logs/adapter-agent/spring.log    
    tail -f logs/alert-bot/spring.log
