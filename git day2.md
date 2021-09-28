# git day2

## * day1 복습내용

> git hub에 push하는 과정 (`add`, `commit`)

```bash
$ git init #저장소 생성
$ git add README.md 
$ git status #항상 확인해주기
$ git commit -m 'Add README.md' #m은 message
```

######                                      ↓           README.md 수정후 

```bash
$ git add README.md
$ git commit -m
#vim이라는 환경 cli환경에서 text편집
```

## * config

> git 설정

	* 기존의 기본 에디터 : `vim` ->visual studio code로 변경
	* 깃허브자료 slide 117 참고
	* vim끄는 단축키 : `esc` + `:`+`w`+`q`

```bash
$ git config --global core.editor "code --wait"
```

## * gitignore

> git으로 관리하지 않을 파일 목록



## * push error

> 원격저장소와 로컬에서의 충돌

 * ##### 원인: 원격저장소 작업이 로컬에 없기 때문에

 * ##### 해결: 다시 push하기 전에 원격저장소 변경사항들과 로컬을 먼저 통합

   ```bash
   $ git pull origin master
   $ git push origin master
   $ git log --oneline
   # ====>***** merge branch 
   ```



## * clone

> git 저장소 복제

* ##### 압축파일과 차이가 있음

  |       압축       |       clone       |
  | :--------------: | :---------------: |
  | 최신 버전의 파일 | git 저장소를 복제 |

  ```bash
  $ git clone https://github.com/gayeon2953/TIL.git
  ```

  

* ##### pull과의 차이

|    pull     |    clone    |
| :---------: | :---------: |
| commit 역할 | 저장소 복제 |

