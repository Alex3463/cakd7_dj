# cakd7_dj

장고 기반 웹 학습입니다.

*깃허브 사용법
github repository 생성

git clone 깃주소 복사 in 원하는 폴더( ex) cakd7_dj )

cd cakd7_dj 폴더로 이동

  <장고 프로젝트 시작>
  bla bla 코드 작성 과정@@@

*변동사항 업데이트 하는법*
git add . : 변경 사항 추가
git commit -m "버젼 명" : 로컬에 변경사항 커밋
git push : 온라인에 변경사항 반영

<장고 프로덱트 생성>
장고 프로젝트 생성 : django-admin startproject do_it_django_prj .
데이터베이스 생성 : python manage.py makemigrations > python manage.py migrate 관리자 계정 생성 : python manage.py createsuperuser
앱 생성 : python manage.py startapp blog single_pages  (각각 생성)
settings.py에 blog 앱과 single_pages 앱 등록
TIME_ZONE 에 'Asia/Seoul' 등록
테이블 모습 확인 : python manage.py runserver
관리자 페이지에서 첫 포스트 작성 blog/admin.py : 관리자 페이지에 post 모델 등록 blog/models.py : Post 모델 정의
표지판 역할 : urls.py
do_it_django_prj/urls.py : 사용자가 웹 방문 시 어떤 페이지로 들어가야 하는지 알려줌 blog/urls.py : urlpatterns 리스트에 url과 url이 들어올 때 어떻게 처리할지 명시