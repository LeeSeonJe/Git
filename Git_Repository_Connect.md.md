# Git Repository Connect
- ##### 단계별로 하나하나씩 스크린샷을 찍은거라 보면서 쭉 따라오면 된다.
- ##### 부가적인 설명은 사진 아래에 적어 놓았습니다.
- ##### 기본적인 workspace setting과 spring project를 생성한 상태에서 진행해야한다.
- ##### 각자 개발 환경이 다르기 때문에 밑에 사진과 완벽하게 같을 수는 없을 것이다.

### Git Bash를 통한 Repository Connect

- ##### 주요 git 명령어
  - git status < 현재 상태를 보여주는 것, 변경사항이 있는 경우 빨간색으로 보여짐
  - git add [fileName || .] < 변경사항을 커밋전에 추가하는 명령어, . 은 전체를 추가하는 것, 추가 후 git status를 할 경우 초록색으로 보여짐
  - git commit -m "[메세지내용]" < 커밋할 때 사용하는 명령어, 메세지내용은 무조건 넣어줘야한다.
  - git remote -v < 연결된 깃을 보는 명령어, 연결을 안 했을경우 아무것도 뜨지 않는다.
  - git remote add origin master < 마스터 브런치로 reqository를 연결하는 명령어
  - git push [-u] origin master < repository에 push하는 명령어

<img width="1019" alt="1" src="https://user-images.githubusercontent.com/59919620/82111167-3fc88200-977e-11ea-8f87-31d69c166c76.png">
<img width="1025" alt="2" src="https://user-images.githubusercontent.com/59919620/82111169-40f9af00-977e-11ea-81e9-5408cb5ffb0d.png">

- git status를 하게 되면 .classPath등과 같은 여러가지 깃에 들어갈 경우 다른 사람과 협업할 때 계속해서 충돌되는 부분이 있을 것이다.
- .gitignore을 통해서 올리지 말아야 할 것을 걸러주자.


<img width="1015" alt="3" src="https://user-images.githubusercontent.com/59919620/82111170-40f9af00-977e-11ea-8642-fef8d910adc6.png">

- vim .gitignore 명령어를 통해서 .gitignore을 생성해 주자. vim은 터미널에서 편집기라고 생각하면 될 것이다.
- 무언가를 쓸 수 있는 곳으로 위치가 변경될 것이다.

======================================================

```

# Created by https://www.gitignore.io/api/java,eclipse
# Edit at https://www.gitignore.io/?templates=java,eclipse

### STS ###
.apt_generated
.classpath
.factorypath
.project
.settings
.springBeans

### Eclipse ###
.metadata
bin/
tmp/
*.tmp
*.bak
*.swp
*~.nib
local.properties
.settings/
.loadpath
.recommenders

# External tool builders
.externalToolBuilders/

# Locally stored "Eclipse launch configurations"
*.launch

# PyDev specific (Python IDE for Eclipse)
*.pydevproject

# CDT-specific (C/C++ Development Tooling)
.cproject

# CDT- autotools
.autotools

# Java annotation processor (APT)
.factorypath

# PDT-specific (PHP Development Tools)
.buildpath

# sbteclipse plugin
.target

# Tern plugin
.tern-project

# TeXlipse plugin
.texlipse

# STS (Spring Tool Suite)
.springBeans

# Code Recommenders
.recommenders/

# Annotation Processing
.apt_generated/

# Scala IDE specific (Scala & Java development for Eclipse)
.cache-main
.scala_dependencies
.worksheet

### Eclipse Patch ###
# Eclipse Core
.project

# JDT-specific (Eclipse Java Development Tools)
.classpath

# Annotation Processing
.apt_generated

.sts4-cache/

### Java ###
# Compiled class file
*.class

# Log file
*.log

# BlueJ files
*.ctxt

# Mobile Tools for Java (J2ME)
.mtj.tmp/

# Package Files #
*.jar
*.war
*.nar
*.ear
*.zip
*.tar.gz
*.rar

# virtual machine crash logs, see http://www.java.com/en/download/help/error_hotspot.xml
hs_err_pid*

# End of https://www.gitignore.io/api/java,eclipse

```

======================================================

- 복사해서 붙여넣어주도록 한다. ctrl+v가 안먹히므로 마우스로 붙여넣어준다. 아니면 shift+insert를 사용해서 붙여준다.

<img width="1014" alt="4" src="https://user-images.githubusercontent.com/59919620/82111171-41924580-977e-11ea-99c0-30b6304142e5.png">
<img width="1015" alt="5" src="https://user-images.githubusercontent.com/59919620/82111172-422adc00-977e-11ea-96f5-38901d03ce23.png">

- 붙여넣기 후 저장을 해야한다. ":wq!" << 로 저장해준다. 콜론부터 다 써야한다. 
- wq로 저장해도 되는데 안될 경우 !를 사용해서 강제로 저장시킨다.

<img width="1018" alt="6" src="https://user-images.githubusercontent.com/59919620/82111174-435c0900-977e-11ea-8020-8f88f1de0637.png">

- git status 명령어를 통해서 확인해 보면 빠진걸 볼 수 있다.

<img width="1013" alt="7" src="https://user-images.githubusercontent.com/59919620/82111175-43f49f80-977e-11ea-8da3-a228fc2e287d.png">

- git add . 명령어로 전체를 add index해준다.
- 약간의 경고가 뜰 것이다. 상관없다.

<img width="1016" alt="8" src="https://user-images.githubusercontent.com/59919620/82111176-43f49f80-977e-11ea-8524-021773805e93.png">

- git status 명령어를 입력하면 초록색으로 변한것을 볼 수 있다.

<img width="1019" alt="9" src="https://user-images.githubusercontent.com/59919620/82111177-448d3600-977e-11ea-9ca9-cbb0fa631ed5.png">

- git commit -m "[메세지내용]" 명령어를 해줘 commit을 해준다. 메세지 내용은 자유롭게 적어준다.

<img width="1045" alt="10" src="https://user-images.githubusercontent.com/59919620/82111178-4525cc80-977e-11ea-8044-d8b9d72e0f56.png">

- 커밋이 완료 후 git status를 입력하면 모든 변경사항이 있는 파일에 대해 올렸기 때문에 clean 하다는 걸 볼 수 있다.

<img width="512" alt="11" src="https://user-images.githubusercontent.com/59919620/82111179-4525cc80-977e-11ea-93f4-9e4c0f5274f9.png">

- 이제 깃으로 돌아가서 repository url을 복사한다.
- git remote add origin RepoURL 을 입력해준다.

<img width="1049" alt="12" src="https://user-images.githubusercontent.com/59919620/82111180-45be6300-977e-11ea-81cc-43c7364ac1f3.png">

- git remote -v 명령어를 통해 연결된 깃을 볼 수 있다.

<img width="1047" alt="13" src="https://user-images.githubusercontent.com/59919620/82111182-4656f980-977e-11ea-9f1e-5484238d123a.png">

- git push [-u] origin master 명령어를 통해서 push한다 u는 생력가능함

<img width="506" alt="14" src="https://user-images.githubusercontent.com/59919620/82111183-46ef9000-977e-11ea-9560-f228fe3e7151.png">

- git으로가서 새로고침하면 파일이 올라간걸 볼 수 있다.


### git repository에 등록 후 이클립스 프로젝트와 연결하기

<img width="826" alt="1" src="https://user-images.githubusercontent.com/59919620/82112350-15c78d80-9787-11ea-976a-8d1912417d98.png">

- 위에 버튼을 누르고 git을 눌러 git perspective를 열어준다

<img width="955" alt="15" src="https://user-images.githubusercontent.com/59919620/82111184-46ef9000-977e-11ea-86e5-f3d9af927415.png">

- 이클립스와 깃을 연결해보자
- add an existing local git repository를 클릭한다.

<img width="1040" alt="16" src="https://user-images.githubusercontent.com/59919620/82111186-47882680-977e-11ea-93a3-e808a0dae73e.png">

- Browse...을 눌러서 프로젝트가 있는 폴더로 설정해준다.

<img width="953" alt="17" src="https://user-images.githubusercontent.com/59919620/82111188-47882680-977e-11ea-8841-567f8073a91c.png">

- 체크박스 후 add 클릭

<img width="955" alt="18" src="https://user-images.githubusercontent.com/59919620/82111189-4820bd00-977e-11ea-9caf-22ce5c9165a7.png">

- 브런치는 아마 master로 되어있을 것이다. 브런치를 변경하도록 한다.

![image](https://user-images.githubusercontent.com/59919620/82112442-f41ad600-9787-11ea-99a5-8b10cf83b224.png)

- 이름은 자유롭게 작성

<img width="953" alt="19" src="https://user-images.githubusercontent.com/59919620/82111190-48b95380-977e-11ea-83ef-971c99e4def8.png">
<img width="953" alt="20" src="https://user-images.githubusercontent.com/59919620/82111191-4951ea00-977e-11ea-9ccb-ed4fedfe1933.png">
<img width="506" alt="21" src="https://user-images.githubusercontent.com/59919620/82111192-49ea8080-977e-11ea-8f05-66afe54a4c51.png">

- home.jsp에서 변경사항 저장 후 커밋시킨다.
