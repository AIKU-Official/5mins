# 5mins - 우리집 고양이도 메리 크리스마스

📢 2024년 2/겨울학기 [AIKU](https://github.com/AIKU-Official) 활동으로 진행한 프로젝트입니다
🎉 2024년 2/겨울학기 AIKU Conference 열심히상 수상!

## 소개
우리집 고양이도 메리 크리스마스!

기존 image editing 모델들의 한계점으로 지적되어 온 것 중 하나는 객체 간의 관계성입니다. 
즉, 특정 객체만을 편집하거나 관계(두 객체의 위치, 크기 등)을 바꾸는 것에서 한계가 있었습니다. 
이번 프로젝트에서는 강아지, 고양이 사진을 크리스마스 분위기로 바꾸는 image editing을 하며 다음 문제를 해결해보고자 합니다. 

- 특정 객체를 추가하거나 수정하는 능력 높이기
- 다양성이 보장된 고품질의 image editing dataset 생성


## 방법론
[데이터셋 생성]
1. 텍스트
   GPT-3.5 turbo 모델을 활용하여 input으로 주어진 instruction 문장을 패러프레이징하여 다양한 instruction 문장 생성
   ![image](https://github.com/user-attachments/assets/7fdac586-9710-46b0-ac69-ed7ea2a49cbf)

2. 이미지
   위에서 생성한 instruction을 랜덤 샘플링하여 이에 맞는 edited image 생성, 이때 instruct pix2pix 모델을 사용하여 paired 데이터셋 생성
   다양한 생성 결과를 위해 image guidance scale을 하나의 값으로 고정하지 않고 여러 값을 사용

   ![image](https://github.com/user-attachments/assets/42cea74b-ae9e-4e93-bc1a-c8edd19c63bb)


## 환경 설정

(Requirements, Anaconda, Docker 등 프로젝트를 사용하는데에 필요한 요구 사항을 나열해주세요)

## 사용 방법

(프로젝트 실행 방법 (명령어 등)을 적어주세요.)

## 예시 결과

(사용 방법을 실행했을 때 나타나는 결과나 시각화 이미지를 보여주세요)

## 팀원

(프로젝트에 참여한 팀원의 이름과 깃헙 프로필 링크, 역할을 작성해주세요)

- [홍길동](홍길동의 github link): (수행한 역할을 나열)
