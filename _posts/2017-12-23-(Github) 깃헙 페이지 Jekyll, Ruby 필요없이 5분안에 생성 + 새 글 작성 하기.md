---
layout: post
title: (Github) 깃헙 페이지 Jekyll, Ruby 필요없이 5분안에 생성 + 새 글 작성 하기
category : Git
date : 2018-03-27
tags : [git, github, github page]
stickie: true
---

# 서론
***
> 누구를 위한것인가?
>
> **Github Page**를 만드려면 `Jekyll`, `Ruby` 등 설치해야 되서 복잡해야 된다고 생각하는 사람
>
> `Github`로 **블로그**를 시작하고 싶은 사람

***
# 단계
***
#### 1. Github 가입
  - https://github.com/

#### 2. Git 프로그램 설치
  - https://git-scm.com/downloads

#### 3. Github 사이트에 로그인 후 Repository 생성
  - https://help.github.com/articles/create-a-repo/   

#### 4. Jekyll Blog Theme 선택 -> Homepage -> Fork
  - http://jekyllthemes.org/

#### 5. Fork 한 Repository의  Repository name 변경
  - `Setting` 클릭
  - `Github아이디.github.io` 입력 (ex. kim.github.io)
  - `Rename` 클릭  

#### 6. Github Page 수정 위해 필요한 절차
  - 폴더를 하나 생성 한다 (폴더 위치 ex.: C:\Users\kim\Desktop\github\blog)
  - `windows 키 + r` -> `cmd` 입력 -> Enter
  - `cd C:\Users\kim\Desktop\github\blog` 입력 -> Enter
  - `git clone http://github.com/사용자깃헙ID/사용자깃헙ID.github.io` 입력 -> Enter
  - clone 한 폴더 에서 아무 파일이나 수정
  - `git add *` 입력 -> Enter
  - `git commit -m "test commit"` 입력 -> Enter
  - `git push origin master` -> Enter -> 로그인 창 뜸 -> 깃헙ID + 비밀번호 입력 (처음 한번만 입력하면 됨)-> Enter

#### 7. 새 글 생성하기
  - C:\Users\kim\Desktop\github\blog에 clone 한 폴더 더블클릭 -> _posts 폴더 더블 클릭
  - 연도-월-일-제목.md (ex.2017-12-25-todo_list.md) 형식으로 파일 생성
  - 참고: md 파일 생성시 `typora`, `haroopad` 와 같은 에디터 사용 하면 편리함

***
# 생성 외 작업
***
#### 1. Github Page 접근하기
  - `Firefox`, `Internet Explorer`, `Chrome`과 같은 인터넷 브라우저를 더블 클릭
  - 주소창 에 `깃헙ID.github.io` 입력 -> Enter

#### 2. Github Page 내용 수정하기 예
  - Link: [example Theme - ProjectGaia](https://github.com/szhielelp/JekyllTheme-ProjectGaia)

  - C:\Users\kim\Desktop\github\blog에 clone 한 폴더 더블클릭 -> _config.yml 파일을 텍스트 에디터로 연다 

  - `baseurl: "/"` 로 수정

  - C:\Users\kim\Desktop\github\blog에 clone 한 폴더 더블클릭 -> 
    _includes 폴더 더블 클릭 -> 수정 하고 싶은 html 파일 선택 후 텍스트 내용 바꾸기

***


#### 참고로 수정을 적용 하려면 수정 후 아래 절차를 꼭 해주어야 함
  - `git add *` 입력 -> Enter
  - `git commit -m "test commit"` 입력 -> Enter
  - `git push origin master` -> Enter -> 로그인 창 뜸 -> 깃헙ID + 비밀번호 입력 (처음 한번만 입력 하면 됨)

