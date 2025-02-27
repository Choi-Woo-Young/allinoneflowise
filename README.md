```markdown
# AllInOneFlowise 설치 방법

0. **Docker & Docker compose 설치**
    맥북용)
    https://www.docker.com/에 접속해서 Download Docker Desktop 버튼 눌러 Apple Silicon 다운받아 설치

1. **allinoneflowise 소스 다운로드**  
   ```bash
   git clone https://github.com/Choi-Woo-Young/allinoneflowise_template.git
   
2. **디렉토리명 수정**  
   `allinoneflowise_template` → `allinoneflowise`

3. **서비스 컨테이너 실행**  
   ```bash
   cd allinoneflowise
   docker compose up --build --watch
   ```

4. **서비스 확인**  
   - **Nginx & Flowise**  
     [http://localhost](http://localhost)  
   - **PostgreSQL & Adminer**  
     [http://localhost:8080/?pgsql=postgres_db&username=postgres&db=flowise_db&ns=public](http://localhost:8080/?pgsql=postgres_db&username=postgres&db=flowise_db&ns=public)
   - **Redis & Redis-Commander**  
     [http://localhost:8081/](http://localhost:8081/)
   - **Chroma**  
     [http://localhost:8000/docs](http://localhost:8000/docs)
   - **Qdrant**  
     [http://localhost:6333/dashboard](http://localhost:6333/dashboard)
```