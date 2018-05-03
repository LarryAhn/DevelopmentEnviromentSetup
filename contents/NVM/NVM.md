# NVM (Node Version Manager)
> 터미널에서 아래 스크립트를 실행한다. 

```
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.11/install.sh | bash
```


> Install 과정을 진행하고 나면 $HOME 에 .nvm 디렉토리가 생성이 되고  
  $HOME/.bash_profile (macOS) / $HOME/.bashrc (linux)에 다음과 같은 환경설정 변수가 추가가 된다.

```
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && . "$NVM_DIR/nvm.sh" # This loads nvm
```


> 터미널 재실행 후 nvm 명령어 사용 가능  

```
# 설치가 가능한 node.js 버전 확인
$ nvm ls-remote

# node.js 설치
$ nvm install {version}

# 해당 버전의 node.js 사용 설정
$ nvm use {version}

# 아래 명령어를 통하여 default node.js 버전 설정 가능
# 터미널을 재실행 했을 때 매 번 nvm use {version}을 하지 않아도 된다.
$ nvm alias default {version}

# node.js 설치 된 리스트 확인
$ nvm list
```
