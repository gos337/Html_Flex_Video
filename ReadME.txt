==============================
           git 설정
==============================
 - gos337@naver.com 계정에 업로드됨
 - 명령어
 <깃 초기화>
 git init   

 <저장소에 연결>
 git remote add origin https://github.com/gos337/Html_Flex_Video.git

 <현재 모든 내용을 깃 버전관리하기 위해서 업로드함>
 git add .

 <"step0 template"로 커밋 생성>
 git commit -m "step0 template"

 <브랜치 생성>
 git branch step0

 <생성된 브랜치 확인>
 git branch -v
  >결과>   * main  5af58d6 step0 template
            step0 5af58d6 step0 template

<모든 브랜치에 파일 업로드>
% git push origin --all



<### 코딩 후....###>
<변경된 파일 확인>
git status
 > 결과 >
    On branch main
    Changes not staged for commit:
    (use "git add <file>..." to update what will be committed)
    (use "git restore <file>..." to discard changes in working directory)
            modified:   .sass-cache/5399f1382284ae2c6c462dfd225f9b0aa3af8216/_reset.scssc
            modified:   .sass-cache/5399f1382284ae2c6c462dfd225f9b0aa3af8216/style.scssc
            modified:   css/style.css
            modified:   css/style.css.map
            modified:   index.html
            modified:   scss/_reset.scss
            modified:   scss/style.scss


 <현재 폴더에서 변경된 모든 파일을 스토리지에 업로드함>
 git add .


<변경된 파일 확인> -> 변경됐던 파일이 수정됨으로 표시됨을 확인 가능 (아직 Git에 업로드는 안됨)
git status
 > 결과 >
    On branch main
    Changes to be committed:
    (use "git restore --staged <file>..." to unstage)
            modified:   .sass-cache/5399f1382284ae2c6c462dfd225f9b0aa3af8216/_reset.scssc
            modified:   .sass-cache/5399f1382284ae2c6c462dfd225f9b0aa3af8216/style.scssc
            new file:   ReadME.txt
            modified:   css/style.css
            modified:   css/style.css.map
            modified:   index.html
            modified:   scss/_reset.scss
            modified:   scss/style.scss

<"전체 UI스타일 완성"로 커밋 생성>
git commit -m "전체 UI스타일 완성" 


<브랜치 생성>
git branch step2

<브랜치 확인>
git branch -v
 > 결과 >
    * main  cc9d8d0 전체 UI스타일 완성
    step0 5af58d6 step0 template
    step2 cc9d8d0 전체 UI스타일 완성

<git에 업로드>
git push origin --all
 > 결과 >
    Enumerating objects: 26, done.
    Counting objects: 100% (26/26), done.
    Delta compression using up to 8 threads
    Compressing objects: 100% (14/14), done.
    Writing objects: 100% (14/14), 12.96 KiB | 4.32 MiB/s, done.
    Total 14 (delta 2), reused 0 (delta 0), pack-reused 0
    remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
    To https://github.com/gos337/Html_Flex_Video.git
    5af58d6..cc9d8d0  main -> main
    * [new branch]      step2 -> step2




============================================================
   SASS 연결
   (_reset.scss 파일에 있는 내용)
   (style.scss 작성 내용을 style.css로 컴파일하기 위한 용도)
============================================================
// sass 명령어
// sass --watch scss/style.scss:css/style.css
// 교제에서는 sass --watch scss/style.scss css/style.css
