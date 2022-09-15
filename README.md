mysite(프로젝트에 해당함 apps의 setting, 도메인의 영역에 해당함)
polls(app에 해당함)

python manage.py migrate
python manage.py makemigrations polls

관리자 id : admin
관리자 password : 1234

## -----------------------------------------------------------------------

Polls/admin.py 에서 아래 코드를 입력해서 admin 에서 데이터를 직접 관리해보는 것 까지 해봄

from django.contrib import admin

from .models import Question

admin.site.register(Question)

## -----------------------------------------------------------------------

작업 진행
뷰 추가하기
뷰가 실제로 뭔가를 하도록 만들기
지름길 : render()
404에러 일으키기
지름길: get_object_or_404()
