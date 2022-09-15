# Delivery Tracker
[![Build Status](https://travis-ci.org/shlee322/delivery-tracker.svg?branch=master)](https://travis-ci.org/shlee322/delivery-tracker)

Delivery and Shipping Tracking Service

## Usage
### Cloud
Document : https://tracker.delivery/guide/

### Self-Hosting

#### Install
```
npm install -g delivery-tracker-apiserver delivery-tracker-client
```

#### Run API Server
```
NODE_ENV=production PORT=8080 delivery-tracker-apiserver
```

#### Run Client (not ready yet)
```
NODE_ENV=production PORT=8888 API_ENDPOINT='http://127.0.0.1:8080' delivery-tracker-client
```

#### Recommend
When using self-hosting, it is recommended to cache APIs and client pages using CDN.

## Information
### License
- Please read the `LICENSE` file.

### Maintainers
- [@shlee322](https://github.com/shlee322)
- [@zinozzino](https://github.com/zinozzino)

### Sponsorship (Enterprise)
We provide sponsors with additional features such as Webhook and Technical Support.
Please contact `contact@tracker.delivery` for more information.



### Sellerhub 환경에 맞게 Build
1. Dockerfile port 9000 변경
2. /root/tracker/delivery-tracker/packages/apiserver 에 들어가서 docker build --tag tracker . 실행
3. docker run -itd --name tracker -p 9000:9000 tracker bash 실행
4. docker exec tracker npm start & 실행



