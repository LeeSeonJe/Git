# Create Spring Project
- ##### 단계별로 하나하나씩 스크린샷을 찍은거라 보면서 쭉 따라오면 된다.
- ##### 부가적인 설명은 사진 아래에 적어 놓았습니다.

## create git Repository
<img width="371" alt="1" src="https://user-images.githubusercontent.com/59919620/82110600-b95e7100-977a-11ea-9fe8-2cc5b84b042b.png">
<img width="505" alt="2" src="https://user-images.githubusercontent.com/59919620/82110601-ba8f9e00-977a-11ea-8ca0-ea2712b8718f.png">

## Create Spring Project
- ### workspace Setting
- ### 새로운 workspace를 만들었을때 가장 기초적인 설정부터 해준다.
<img width="911" alt="3" src="https://user-images.githubusercontent.com/59919620/82110602-bb283480-977a-11ea-8ff6-3fa4ddf9c369.png">
<img width="596" alt="4" src="https://user-images.githubusercontent.com/59919620/82110603-bbc0cb00-977a-11ea-816d-50cc136bcb6d.png">
<img width="598" alt="5" src="https://user-images.githubusercontent.com/59919620/82110604-bbc0cb00-977a-11ea-8115-19458389bf64.png">
<img width="608" alt="6" src="https://user-images.githubusercontent.com/59919620/82110605-bc596180-977a-11ea-8d2c-dbd86a6e6170.png">
<img width="595" alt="7" src="https://user-images.githubusercontent.com/59919620/82110606-bc596180-977a-11ea-9cee-81a7df14a835.png">
<img width="609" alt="8" src="https://user-images.githubusercontent.com/59919620/82110607-bcf1f800-977a-11ea-99d3-fd9a9e67f692.png">
<img width="590" alt="9" src="https://user-images.githubusercontent.com/59919620/82110608-bcf1f800-977a-11ea-84e2-6a0a723e61a5.png">
<img width="596" alt="10" src="https://user-images.githubusercontent.com/59919620/82110609-bd8a8e80-977a-11ea-93d1-105b037ed22d.png">
<img width="593" alt="11" src="https://user-images.githubusercontent.com/59919620/82110610-bd8a8e80-977a-11ea-8e30-6e0fc5c60e92.png">
<img width="1004" alt="26" src="https://user-images.githubusercontent.com/59919620/82110627-c3806f80-977a-11ea-8d9c-c225dd4949a8.png">

- 마지막은 Maven 설정입니다. 스크린샷을 늦게 찍어서 조금 다름
- Maven 관련 설정은 [Maven Setting](https://github.com/LeeSeonJe/Spring) 을 참고

## New Server
<img width="920" alt="12" src="https://user-images.githubusercontent.com/59919620/82110611-be232500-977a-11ea-85f2-599b6f752cb3.png">
<img width="1109" alt="13" src="https://user-images.githubusercontent.com/59919620/82110612-bebbbb80-977a-11ea-8196-48bddac9f60a.png">
<img width="730" alt="14" src="https://user-images.githubusercontent.com/59919620/82110613-bf545200-977a-11ea-9fc3-04e3ffc29d0d.png">

## Create Spring Project
<img width="929" alt="15" src="https://user-images.githubusercontent.com/59919620/82110614-bf545200-977a-11ea-959a-35125dc80711.png">
<img width="920" alt="16" src="https://user-images.githubusercontent.com/59919620/82110615-bfece880-977a-11ea-9c68-bc2a428a2889.png">
<img width="500" alt="17" src="https://user-images.githubusercontent.com/59919620/82110616-bfece880-977a-11ea-8156-59802c920249.png">
<img width="926" alt="18" src="https://user-images.githubusercontent.com/59919620/82110617-c0857f00-977a-11ea-8217-e1df689dda3a.png">
<img width="926" alt="19" src="https://user-images.githubusercontent.com/59919620/82110618-c11e1580-977a-11ea-8924-464965b50ae3.png">

- 프로그래스바를 보면서 완료되기를 기다려줍니다.

## Fit-Version
- ### project properties를 연다.

<img width="916" alt="20" src="https://user-images.githubusercontent.com/59919620/82110619-c11e1580-977a-11ea-81eb-f9798d7fbcd3.png">
<img width="916" alt="21" src="https://user-images.githubusercontent.com/59919620/82110620-c1b6ac00-977a-11ea-875f-bed2ce2d6ae0.png">
<img width="264" alt="22" src="https://user-images.githubusercontent.com/59919620/82110621-c1b6ac00-977a-11ea-82f9-b6ad962b22da.png">

- 옆에 explorer을 보게되면 조금 변화된거를 볼 수 있다. 처음에는 1.6버전으로 되어있는데 1.8로 바뀌었을것

<img width="254" alt="23" src="https://user-images.githubusercontent.com/59919620/82110623-c24f4280-977a-11ea-8731-ec12c8320e70.png">

- 설정을 하다보면 이런 에러가 뜨는 것을 확인할 수 있다.
- 우선 무시하고 버전 세팅이 끝난 후 workspace를 재실행하면 안뜰 것이다.
- 뜨는 이유는 workspace .metadata > .log 파일 때문에 뜬다고 한다.

<img width="911" alt="24" src="https://user-images.githubusercontent.com/59919620/82110625-c24f4280-977a-11ea-9339-e7d9ac27ad7a.png">
<img width="918" alt="25" src="https://user-images.githubusercontent.com/59919620/82110626-c2e7d900-977a-11ea-9915-8a043a525ec0.png">

## root-context 위치 변경

<img width="268" alt="27" src="https://user-images.githubusercontent.com/59919620/82110628-c3806f80-977a-11ea-839f-cc432d92db7f.png">
<img width="904" alt="28" src="https://user-images.githubusercontent.com/59919620/82110629-c4190600-977a-11ea-9ae5-8a74f99d326f.png">

- web.xml에 /WEB-INF/!!/@@/##/$$/root-context.xml > classPath:root-context.xml로 
