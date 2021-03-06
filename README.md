# Lv01-02
임베디드 스쿨 2기 - 레벨 1 

# 가장 우선 해야할 것

0. USB 용 시동디스크 만들기
1. 리눅스 설치(멀티 부팅 되게 설치하셔도 좋아요) - Version: Ubuntu 20.04 로 부탁드립니다.   
2. 멀티 부팅이 싫다면 그냥 전체를 리눅스로 설치해도 무방합니다.  
3. 요즘은 웹 브라우저용 공인 인증서가 있어서 리눅스로도 뱅킹이 가능합니다.    
4. 리눅스에 한글 설정하기(필요하다면 수업시간에 같이 진행해봅니다)  

## Ubuntu 이미지 다운 받는 장소
```make
https://ubuntu.com/download/desktop
```

## USB 시동 디스크 만드는 프로그램 다운로드 장소
```make
https://universal-usb-installer.kr.uptodown.com/windows
```

## 멀티부팅을 원할 경우

1. 파티션 분할이 되어 있어야 합니다.  
2. 분할된 파티션에 파일 시스템이 할당되어 있으면 안되고 아무것도 없는 상태로 만들어줘야 합니다.  
3. 최종 리눅스 설치시 alongside 라는 메시지가 나올텐데 이것이 나오면 멀티부팅이 선택된 것이고 나오지 않는다면 파티션 분할이 안되었거나 다른 문제가 발생한것이니 확인해보고 진행해주세요.  

## 주의할점

1. 파티션 분할이 제대로 되지 않은 상태에서 혹은 alongside가 나오지 않는 상황에서 진행하면 윈도우를 밀어버릴 수 있습니다. 실수를 대비하여 중요한 데이터는 반드시 외장 하드등에 백업을 해주세요.  

## 설치시 발생하는 문제점들

1. LG 노트북의 경우 리눅스 설치가 매우 어려울 수 있습니다.  
2. 리눅스 노트북으로 추천은 Dell 혹은 Lenovo를 추천드립니다.  
3. 자금에 여유가 없으신 분들은 삼성 노트북도 나쁘지 않습니다.  
4. 현재 어쩔 수 없이 LG 노트북을 사용하셔야 하는 분의 경우엔 Virtual Box를 사용해서 Ubuntu 리눅스를 설치하면 될 것 같습니다.  
5. BIOS 설정시 발생할 수 있는 문제점으로 Secure Boot 등이 있는데 만약 USB 시동 디스크 인식이 잘 되지 않으면 카톡등을 통해 질문해주시면 감사하겠습니다.  

# 리눅스 설치 후 진행할 내용

## 업데이트 받기
```make
sudo apt-get update
sudo apt-get install vim
sudo apt-get install build-essential
sudo apt-get install git
```

## 학습 저장소 다운 받기
```make
mkdir proj
cd proj
git clone https://github.com/EmbeddedSchoolRepo/Lv01-02.git
cd Lv01-02
ls
```

## 현재 저장소의 상태를 확인하는 방법
```make
git status
```

## 저장소에 추가한 내용 혹은 변경 내역을 적용하는 방법
```make
git add (추가한내용)           필요하다면
git commit -am "작업한 내용에 대한 간략한 메시지를 기록합니다."
git push origin main
```

## 실제 수강생분들의 경우엔 fork를 해서 진행해야합니다.
```make
이 부분에 대해서는 첫날 수업시간에 리눅스가 설치된 노트북을 활용해서 같이 진행해보도록 하겠습니다.
```

## 수업 진행 방식
```make
1. 지금처럼 선생님은 사무실에 들어가서 스트리밍을 진행합니다.
2. 3인 오프라인 1인 온라인 형식으로 로테이션을 돕니다.

논의 결과: 수업 방식은 1번 방식을 채택하여 진행합니다.
```
