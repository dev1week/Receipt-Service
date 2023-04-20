### 소개


![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/98fb2e89-03a9-49b7-81f7-8eebf89dfe80/Untitled.png)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/9d2d21a2-260f-4912-8c4d-230c19a9f76a/Untitled.png)

네이버 클라우드 OCR을 활용하여 가계부 웹앱을 제작하였습니다. 

###제공하는 기능
1. 사용자가 영수증 이미지를 업로드하면 영수증의 내용을 글자로 변환합니다.
2. 영수증 데이터를 종합하여 가계부 형식으로 재가공하는 기능을 수행합니다. 

### Demo

**⇒ [Demo Link](https://github.com/dev1week/Receipt-App-Server)**

### Stack

- `**Django Rest Framework` , `React` , `Docker`,`NaverCloud`**

### Role

**영수증 도메인 API 구축 `Django Rest Framework`**

**⇒  [Git](https://github.com/dev1week/Receipt-App-Server)**

- **네이버 클라우드에서 제공하는 OCR API 활용 및 Custom API 제작**
    1. 사진을 multipart로 전송 받는 로직 구현 
    2. 전송받은 사진 정보를 바탕으로 OCR API가 요구하는 요청에 맞도록  json body 생성 로직 구현 
    3. 네이버 클라우드 ocr api를 통해 분석된 내용을 Db에 저장하는 로직 구현
    4. DB 내 데이터 CRUD API 구현 

**영수증 인식 프론트 구축 `React`**

**⇒  [Git](https://github.com/dev1week/Reciept-React)**

1. 연도별 필터링 기능 
2. 필터링한 연도내 각 월별 비용 그래프 구현 
3. 양식 입력창 숨기기 보이기 버튼 구현
4. Django Rest Frame work api 연동 
5. Multipart 이용 사진 전송 기능 구현 

**Docker 활용 네이버 클라우드 서버 플랫폼에서 배포 경험**

- requirements.txt 추출 후 도커 파일과 이미지 생성, 이미지 도커 허브에 등록
- 로컬에서 도커 이미지 빌드 테스트 후 네이버 클라우드에서 도커 활용 배포
