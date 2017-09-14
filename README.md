[![PyPi Version](https://img.shields.io/pypi/v/django-multi-captcha-admin.svg)](https://pypi.python.org/pypi/django-multi-captcha-admin)
[![GitHub stars](https://img.shields.io/github/stars/a-roomana/django-multi-captcha-admin.svg?style=social)](https://github.com/a-roomana/django-multi-captcha-admin)
# django-multi-captcha-admin

easy added captcha to login page of django admin

----------
## Dependency

To use this module you need to install django and one of the captcha engines, which you can install it with easy_install or pip.

----------
## Installation

    pip install django-multi-captcha-admin   

----------
## Usage

settings.py
```python
INSTALLED_APPS = [
	...
	'multi_captcha_admin',
	'django.contrib.admin',
	...
]
```

command
```bash
pip install [django-simple-captcha | django-recaptcha | django-recaptcha2]
```
----------
**Engines**

We support three famous engines to render CAPTCHA. You need to install one of them, then add it to your django project according to their documents.

 - [simple-captcha](https://github.com/mbi/django-simple-captcha)
 - [recaptcha](https://github.com/praekelt/django-recaptcha)
 - [recaptcha2](https://github.com/kbytesys/django-recaptcha2)

For more information, please go to the engine site.

----------
## Example

After installing the desired engine, add the following to your `settings.py` with the name of the installed engine:

```python
MULTI_CAPTCHA_ADMIN = {
    'engine': 'recaptcha2',
}
```

----------
## Results

[recaptcha2](https://github.com/kbytesys/django-recaptcha2)

![captcha of recaptcha2](http://bayanbox.ir/view/2417903076718397977/reCaptcha2.png)


[recaptcha](https://github.com/praekelt/django-recaptcha)

![captcha of recaptcha](http://bayanbox.ir/view/2014387201108001651/reCaptcha.png)


[simple captcha](https://github.com/mbi/django-simple-captcha)

![captcha of recaptcha](http://bayanbox.ir/view/721684099022571779/simple-captcha.png)
