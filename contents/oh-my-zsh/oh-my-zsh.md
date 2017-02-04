# oh-my-zsh

> zsh 설치 확인

```
$ zsh --version
zsh 5.0.8 (x86_64-apple-darwin15.0)  
```  
  
> 설치가 되어 있지 않다면 brew를 통해 zsh 를 설치 한다.

```
$ brew update
$ brew install zsh
```  
  
> 기본 쉘 zsh 로 변경하기

```
$ which zsh
/bin/zsh
$ chsh -s `which zsh`
```
  
> Install oh-my-zsh

```
$ sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```
