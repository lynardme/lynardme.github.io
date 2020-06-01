---
layout: "post"
title: "Django framework"
date: 2020-05-30
category: devtips
tags: [django, python]
---

#### Commands
``` python
django-admin startproject <nameofproject>
django-admin startapp <nameofapp>
```

#### Migration
``` 
python manage.py makemigrations polls        
python manage.py migrate
```

#### Shell
```
> python manage.py shell

from polls.models import Question, Choice
from django.utils import timezone
q = Question(question_text="What is your favorite python framework?", pub_date=timezone.now())
q.save()
q.id

Query all
Question.objects.all()

Filter
Question.objects.filter(id=1)
Question.objects.get(pk=1)

Add data in reference table
q = Question.objects.get(pk=1)
q.choice_set.all()
q.choice_set.create(choice_text="Django", votes=0)
q.choice_set.create(choice_text="Flask", votes=0)
q.choice_set.create(choice_text="Web2py", votes=0)


Manage Admin
python manage.py createsuperuser
```