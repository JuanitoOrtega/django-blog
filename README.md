#### Video Tutorial for this project
https://youtu.be/SQ4A7Q6_md8
<br><br>

#### Getting the files
Download zip file<br> 
or <br>
git clone command (need git to be installed) and remove git folder afterwards
```shell
git clone https://github.com/andyjud/django-starter.git . && rm -rf .git
```

## Setup

#### - Create Virtual Environment
###### # Mac
```shell
python3 -m venv venv
source venv/bin/activate
```

###### # Windows
```shell
python3 -m venv venv
.\venv\Scripts\activate.bat
```

#### - Install dependencies
```shell
pip install --upgrade pip
pip install -r requirements.txt
```

#### - Migrate to database
```shell
python manage.py migrate
python manage.py createsuperuser
```

#### - Run application
```shell
python manage.py runserver
```

#### - Generate Secret Key ( ! Important for deployment ! )
```shell
python manage.py shell
from django.core.management.utils import get_random_secret_key
print(get_random_secret_key())
exit()
```

### - Update index
```shell
python manage.py update_index
```
