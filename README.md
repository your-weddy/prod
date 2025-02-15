#### 배포용 레포 클론
```
git clone --recursive  https://github.com/your-weddy/prod.git
```
#### 클론한 파일로 이동 후
```
docker-compose -f docker-compose.backend.dev.yml up
```

#### front레포와 back 레포가 최신 main브랜치가 아닐 떄 업데이트 법
```
cd prod
git submodule update --remote --merge
git commit -m "chore: 서브모듈을 업데이트한다"
git push origin main
```
