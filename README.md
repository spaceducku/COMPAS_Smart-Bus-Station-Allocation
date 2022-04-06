# COMPAS_Smart-Bus-Station-Allocation
2021 LH COMPAS 국토도시분석과제 : 수원시 스마트 버스정류장 입지선정(우수상, 94팀 참가)
[[Link]](https://compas.lh.or.kr/subj/past/code-report?subjNo=SBJ_2102_002&teamNo=1178)

![image](https://user-images.githubusercontent.com/59859965/161897386-d24b95c1-6f78-4524-a548-bedee9e0656f.png)


[[분석코드 확인하기]](https://compas.lh.or.kr/subj/past/code?subjNo=SBJ_2102_002&teamNo=1178)


## 분석과제

#### 미세먼지 등 대기정보 수집 및 제공과 일반시민의 접근성‧편의성 등 공공적 요소와 예산 절감 등을 위한 상업광고 등을 고려하여 수원시 내 스마트 버스정류장 우선 설치위치 30개소 제시(BIS 설치 가능 장소 고려)

![image](https://user-images.githubusercontent.com/59859965/161898678-75e5ce4d-2c21-4964-9055-a4070cf8ad0d.png)


## 설치요건 정의

![image](https://user-images.githubusercontent.com/59859965/161899758-003b2e11-8013-4403-9171-75d179626da1.png)



## EDA(수원시 현황 분석)

![image](https://user-images.githubusercontent.com/59859965/161899164-c488e7ff-237c-4d27-8084-3f4b604623b0.png)
![image](https://user-images.githubusercontent.com/59859965/161899203-d6a1ec76-035c-489f-ba7d-a686b4a1b4c9.png)
![image](https://user-images.githubusercontent.com/59859965/161899292-4c3333fe-aac2-4e83-a7fe-d0e121059078.png)
![image](https://user-images.githubusercontent.com/59859965/161899378-8e295729-6717-4c5d-8800-76f4b6553e76.png)
![image](https://user-images.githubusercontent.com/59859965/161899414-ff08142c-b411-41be-8f07-4791fff79fb2.png)
![image](https://user-images.githubusercontent.com/59859965/161899441-c865b728-9d64-406d-b1da-7e8b73017b67.png)

## 가변거리버퍼를 이용한 전처리

![image](https://user-images.githubusercontent.com/59859965/161900291-e1efb8b5-b3b1-42b9-beae-065951e80906.png)


## 입지선정지수 분석

#### 1. 인구수
![image](https://user-images.githubusercontent.com/59859965/161901524-b73f9209-02cc-40ec-b83f-77309cb8d264.png)

![image](https://user-images.githubusercontent.com/59859965/161897669-1b661a6b-e262-4d82-98c8-881026096ca3.png)

![image](https://user-images.githubusercontent.com/59859965/161901570-fe4f50c3-e884-4547-b907-b1c76690689e.png)


#### 2. 대기오염도
![image](https://user-images.githubusercontent.com/59859965/161901777-6fc444ee-f8e2-4e23-9f58-6304df7e2d3a.png)

![image](https://user-images.githubusercontent.com/59859965/161901824-53827b66-88eb-4ffd-8fb8-6cb3aaa9bacf.png)

![image](https://user-images.githubusercontent.com/59859965/161901860-dde5da43-13d6-4d6c-b25b-17990f303d15.png)

![image](https://user-images.githubusercontent.com/59859965/161898306-2ad8a7c5-451f-4b48-91a3-d156646ac9a4.png)


#### 3. 광고효과


![image](https://user-images.githubusercontent.com/59859965/161898011-ff969c36-13b8-40bf-a642-750d354b84c8.png)

![image](https://user-images.githubusercontent.com/59859965/161898046-89ee95a9-7acc-4ffd-9b2a-caa72dbba788.png)

![image](https://user-images.githubusercontent.com/59859965/161900439-8ba29e45-d6d1-4a93-a7e7-84a7243ef0da.png)


## RBS 정규화 및 MCLP 최적화

#### 1. RobustScale 정규화

![image](https://user-images.githubusercontent.com/59859965/161900980-99514e7e-f5f5-45c3-9e44-3069cf132da7.png)
![image](https://user-images.githubusercontent.com/59859965/161901015-e25425ad-c600-4353-9d24-5a6cabd429a3.png)

#### 2. Maximal Covering Location Problem 최적화

![image](https://user-images.githubusercontent.com/59859965/161901147-b7c6f2ef-f349-462a-8fb1-8f2d60e15146.png)

#### 3. Greedy Adding Algorithm with Substitution procedure 적용

![image](https://user-images.githubusercontent.com/59859965/161901313-2cbc34b7-7ce9-4519-8fce-ad7ee3f61259.png)
![image](https://user-images.githubusercontent.com/59859965/161901355-19c80390-fa4a-4ab1-8ee8-8514ec52076e.png)


## 최종입지선정 결과

#### 입지선정지수별 시각화

![image](https://user-images.githubusercontent.com/59859965/161896599-6463b604-ca72-46d8-9d70-199a25f36873.png)


#### 최종 후보지 선정
![image](https://user-images.githubusercontent.com/59859965/161896695-fe6a0ae4-6c9f-45a6-ab54-3ef32364b79b.png)

## 참고문헌 및 외부데이터

![image](https://user-images.githubusercontent.com/59859965/161900685-0c28c748-6ec6-4573-81eb-35c5894be5a9.png)
