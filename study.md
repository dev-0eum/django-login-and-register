## Reference Site
[text](https://www.inflearn.com/course/%EC%9E%A5%EA%B3%A0-%ED%95%80%ED%84%B0%EB%A0%88%EC%8A%A4%ED%8A%B8)

## MVC Structure
Model
View
Templete(Controller)

## Routing
from django.urls import path
urls.py
urlpatterns = [
    path("log-in/",LogInView.as_view(), name="log_in")
]
>> localhost:8080/accounts/log-in

from django.contrib import admin
urlpatterns = [
    path("admin/", admin.site.urls),
    path("accounts/", include('accounts.urls')),
] >> accounts 앱의 urls 디렉터리 하위 구조로 변경한다.




git ignore > 7강