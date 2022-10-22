# Microsoft-Azure
This space is to record different API services in Microsoft Azure
## Index.
1. [Computer Vision](#1-computer-vision)
2. [Face API](#2-face-api)
3. [Custom Vision](#3-custom-vision)
4. [OCR](#4-ocroptical-character-recognition)
5. [Virtual Machine](#5-virtual-machine)<br>
    5.1. [VM에서 Window환경 구축](#51-azure-virtual-machine에서-window-실행하기-관련-링크)<br>
    5.2. [VM에서 Ubuntu환경 구축](#52-azure-virtual-machine에서-ubuntu-실행하기-관련-링크)<br>
    5.3. [VM 확장 집합](#53-azure에서-가상머신-확장-집합-만들기-관련-링크)<br>
<hr>
<!-- 5. [여기]() -->

## 1. Computer Vision 
    [1]  + 리소스 만들기
    [2] 'Computer Vision' 만들기 선택
    [3] <기본 사항> : 자신의 리소스그룹 선택
        <태그> : 태그 별로 따로 분류해서 비용이 얼마나 나오는지 구분 가능
    [4] 검토 + 만들기

### Computer Vision API를 이용한 Demo List.
1) Descprtion : 이미지 설명 ([Code 링크](), [관련 링크]('https://learn.microsoft.com/ko-kr/azure/cognitive-services/computer-vision/concept-describing-images'))<br>
    #### Input.
    <img src ='https://img0.yna.co.kr/etc/inner/KR/2016/10/29/AKR20161029046000004_01_i_P2.jpg' style='width: 400px; height: 220px'></img>
    #### Output.     
    <img src ='./Result/1_description.PNG'></img>
<br>

2) Object Detection : Image 속에 있는 object을 감지하고 boxing하는 데모 ([Code 링크](), [관련 링크]('https://learn.microsoft.com/ko-kr/azure/cognitive-services/computer-vision/concept-tagging-images'))
    #### Input.
    <img src ='https://mblogthumb-phinf.pstatic.net/MjAyMDA5MDdfMjQ1/MDAxNTk5NDY1MjUxMjM4.zbBfDyquP67Utlw2d6pFOtHqnJyfkukH3PTDgDTg8Zkg.qQWiX02sgIaExMrU-guWXKDRsmnGBBxeS_bz2Ioy8YUg.PNG.vet6390/%EA%B0%95%EC%95%84%EC%A7%80_%EA%B3%A0%EC%96%91%EC%9D%B4_%ED%95%A8%EA%BB%98_%ED%82%A4%EC%9A%B0%EA%B8%B0.PNG?type=w800' style='width: 400px; height: 280px'></img><br>
    #### Output.     
    <img src ='./Result/2_object_detection.PNG' style='width: 400px; height: 280px'></img>
<hr>

## 2. Face API
    [1]  + 리소스 만들기
    [2] 'Face' 만들기 선택
    [3] <기본 사항> : 자신의 리소스그룹 선택
        <태그> : 주제에 따라 분류 및 비용 확인 가능
    [4] 검토 + 만들기
### Face API를 이용한 Demo List.
1) Face Recognition: 이미지에서 얼굴을 인식하는 데모 ([Code 링크](), [관련 링크]('https://learn.microsoft.com/ko-kr/azure/cognitive-services/computer-vision/concept-face-detection'))
    #### Input.
    <img src ='./Result/3_face_input.PNG' style='width: 400px; height: 280px'></img><br>
    #### Output.     
    <img src ='./Result/3_face_output.PNG' style='width: 400px; height: 280px'></img><br>

<hr>

## 3. Custom Vision
    [1]  + 리소스 만들기
    [2] 'Custom Vision' 만들기 선택
    [3] <기본 사항> : 만들기 옵션 > 사용자에 need에 따라 "예측/학습" 선택 
    [4] 검토 + 만들기
    [5] 리소스를 만든 후 Custom Vision 리소스 그룹을 이동 후 2번째 옵션에 있는 "Custom Vision Portal"을 클릭
    [6] MS 계정으로 로그인 후 Project를 만들고 사용
        - Classification Model (Multi-label/Multi-class) 
        - Object Detection
### Custom Vision를 이용한 Demo List.
1) 3가지 Category(짜장면, 짬뽕, 탕수육)를 구분하는 예측 모델 ([Code 링크](), [관련 링크]('https://learn.microsoft.com/ko-kr/azure/cognitive-services/custom-vision-service/getting-started-build-a-classifier'))
    #### Input.
    #### - 짜장면
    <img src ='https://t3.ftcdn.net/jpg/04/99/47/46/360_F_499474623_E54OAKrMbnUdZPqgg6hG8aVSV0M0KyR2.jpg' style='width: 400px; height: 280px'></img><br>
    #### - 탕수육
    <img src ='https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQnjs2tjmaVpAVeCJ-ePRlYPpobkVdnqkv6sA&usqp=CAU' style='width: 400px; height: 280px'></img><br>
    #### - 짬짜면
    <img src ='https://image.ytn.co.kr/general/jpg/2016/0802/201608020600065468_d.jpg' style='width: 400px; height: 280px'></img><br>
    #### Output.     
    <img src ='./Result/4_custom_vision_multiclass.PNG'></img><br>

<hr>

## 4. OCR(Optical Character Recognition)
    [1]  + 리소스 만들기
    [2] 'Custom Vision' 만들기 선택
    [3] <기본 사항> : 만들기 옵션 > 사용자에 need에 따라 "예측/학습" 선택 
    [4] 검토 + 만들기
### OCR를 이용한 Demo List.
1) OCR API를 이용해 이미지에 있는 문자 읽기 ([Code 링크](), [관련 링크]('https://learn.microsoft.com/ko-kr/azure/cognitive-services/computer-vision/overview-ocr'))
    #### Input.
    <img src ='./Result/3_face_input.PNG' style='width: 400px; height: 280px'></img><br>
    #### Output.     
    <img src ='./Result/3_face_output.PNG' style='width: 400px; height: 280px'></img><br>
<hr>

## 5. Virtual Machine
### 5.1. Azure Virtual Machine에서 Window 실행하기 ([관련 링크](https://learn.microsoft.com/ko-kr/azure/virtual-machines/windows/quick-create-portal))
#### 1) Virtual Machine 만들기
    [1]  + 리소스 만들기
    [2] 'Virtual Machine' 만들기 선택
    [3] <기본 사항>
            가상머신이름 >> 사용자 임의로 설정
            이미지 >> "Windows Sever 2022" 선택
            관리자계정 >> "이름", "암호" 설정 후
            인바운드 포트 >> HTTP(80) 추가
    [4] 검토 + 만들기 : 가상머신 생성
#### 2) Virtual Machine 연결하기
    [1] Window에 "원격 데스크톱 연결"을 검색후 Azure의 "공용 IP 주소" 입력
    [2] 이전에 가상머신 생성 시 입력했던 "이름"과 "암호" 입력
    [3] 가상 머신에서 Window 생성완료
    [4] 가상 머신의 Window에서 powershell 실행 후 "Install-WindowsFeature -name Web-Server -IncludeManagementTools" 입력 : 기본 설치
    [5] chrome열고 "공용ip주소" 입력 시 사이트가 뜨면 성공

### 5.2. Azure Virtual Machine에서 Ubuntu 실행하기 ([관련 링크](https://learn.microsoft.com/ko-kr/azure/virtual-machines/linux/quick-create-portal))
    [1] + 리소스 만들기
    [2] 'Virtual Machine' 만들기 선택
    [3] <기본 사항>
            가상머신이름 : 설정
            이미지 : "Ubuntu 18.04" 선택
            인증유형 : "SSH 공개 키" 설정
            관리자계정 : "이름", "암호" 설정 후
            인바운드 포트 >> HTTP(80) 추가
    [4] 검토 + 만들기
#### 2) Virtual Machine 연결하기
    [1] CMD를 실행시킨 후 
        ssh "가상머신이름"@"공용ip주소" 입력 후 비밀번호 입력
    [2] 가상 머신에서 Ubuntu 연결 완료
    [3] cmd에서 "sudo apt-get -y update" 
                "sudo apt-get -y install nginx" 입력
    [4] chrome열고 "공용ip주소" 입력 시 사이트가 뜨면 성공
        
### 5.3. Azure에서 가상머신 확장 집합 만들기 ([관련 링크](https://learn.microsoft.com/ko-kr/azure/virtual-machine-scale-sets/quick-create-portal))


