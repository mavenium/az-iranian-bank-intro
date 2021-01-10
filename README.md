<!--![GitHub All Releases](https://img.shields.io/github/downloads/ali-zahedi/az-iranian-bank-intro/total)-->
<!--![GitHub issues](https://img.shields.io/github/issues/ali-zahedi/az-iranian-bank-intro)-->
![GitHub](https://img.shields.io/github/license/ali-zahedi/az-iranian-bank-intro)
![GitHub](https://img.shields.io/pypi/pyversions/az-iranian-bank-intro.svg?maxAge=2592000)
![GitHub](https://img.shields.io/pypi/v/az-iranian-bank-intro.svg?maxAge=2592000)

# AZ Iranian Bank intro

<p dir="rtl">
 کدهای آزاد و متن باز به زبان پایتون (python) که برای استفاده از اطلاعات، اعتبار سنجی درگاه های بانکهای ایرانی توسعه داده شده است.
</p>

🌟 If you ❤️ library, please star it! 🌟

[[_TOC_]]


<h1 dir="rtl">نصب</h1>

<p dir="rtl"> نصب از طریق پکیج منیجر </p>

```pip install az-iranian-bank-intro```


<h1 dir="rtl">نحوه استفاده</h1>

<h2 dir="rtl">اعتبار سنجی کارت ها</h2>

<p dir="rtl">
برای اعتبار سنجی کارت های بانکی کافی است متد اعتبار سنجی را ایمپورت کنیم و شماره کارت مورد نظر را به آن پاس دهیم. در صورتی که شماره کارت مورد نظر معتبر باشد برنامه به کار خود ادامه خواهد داد و در صورتی که نا معتبر باشد exception ارسال خواهد شد. 
</p>

```python
import logging
from azbankintro import card_validate, CardValidationException

try:
    card_validate('6280992042433333')
    logging.debug('کارت معتبر است.')     
except CardValidationException:
    logging.debug('کارت نا معتبر است.')
```


# TODO

- [ ] Documentation

- [ ] Bank list

- [ ] Logo

- [ ] Validate card 

- [ ] Validate IBAN



## توسعه

<p dir="rtl">
 اگر از این بسته استفاده می کنید و خوشتون اومده با دادن ستاره به ما دلگرمی بدید.البته که اگر زمان بگذارید و گسترش بدید خیلی استقبال می کنیم و خوشحال میشیم. البته که در هیچ کدوم از این موارد اصراری نیست. 
</p>
<p dir="rtl">
 شاد باشید و خندون
</p>

## License

The MIT License (MIT). Please see [License File](LICENSE) for more information.
