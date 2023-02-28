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



============================================================
   SASS 연결
   (_reset.scss 파일에 있는 내용)
   (style.scss 작성 내용을 style.css로 컴파일하기 위한 용도)
============================================================
// sass 명령어
// sass --watch scss/style.scss:css/style.css
// 교제에서는 sass --watch scss/style.scss css/style.css
