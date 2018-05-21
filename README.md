# django-practice

last practice: 5/13/18, left off @ https://docs.djangoproject.com/en/2.0/intro/tutorial05/
start of lesson

djangoadmin

ex. of accessing the django-admin shell w/ manage.py:

`Carlys-MacBook-Pro-2:mysite carlylanglois$ python3 manage.py shell
Python 3.6.5 (v3.6.5:f59c0932b4, Mar 28 2018, 03:03:55)
[GCC 4.2.1 (Apple Inc. build 5666) (dot 3)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
(InteractiveConsole)
>>> import datetime
>>> from django.utils import timezone
>>> from polls.models import Question
>>> future_question = Question(pub_date=timezone.now() + datetime.timedelta(days=30))
>>> future_question.was_published_recently()
True
>>>`
