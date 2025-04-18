# Angular Sample Project

## install
``` shell
npm install
```

## Start
``` shell
npm run start

# or

ng serve
```

## 기본 포트
- 4200

## dockerizing

### node 18
- Image build
``` shell
docker build -t sample-angular-started-node18:latest -f node.js18:angular.Dockerfile .
```

- Container run
``` shell
docker run -p 4200:4200 \
  --name angular18 sample-angular-started-node18 ng serve --host 0.0.0.0
```

### node 20
- Image build
``` shell
docker build -t sample-angular-started-node20:latest -f node.js20:angular.Dockerfile .
```

- Container run
``` shell
docker run -p 4200:4200 \
  --name angular20 sample-angular-started-node20 ng serve --host 0.0.0.0
```

README from
