=====================
django_localflavor_cn
=====================

Country-specific Django helpers for China.

=======
WARNING
=======

This app has been superseded by the newly created django-localflavor_ app
which recombines all the different country locaflavors again (after having
been removed from Django). Development and maintenance of this app has
stopped and is only left online as a reminder for the users of those apps.
It will be removed after grace period of 1 Django release (~spring 2014).

.. _django-localflavor: https://github.com/django/django-localflavor/

What's in the China localflavor?
=================================

* forms.CNProvinceSelect: A ``Select`` widget that uses a list of Chinese
  regions as its choices.

* forms.CNPostCodeField: A form field that validates input as a Chinese post
  code. Valid formats are XXXXXX where X is digit.

* forms.CNIDCardField: A form field that validates input as a Chinese
  Identification Card Number. Both 1st and 2nd generation ID Card Number are
  validated.

* forms.CNPhoneNumberField: A form field that validates input as a Chinese
  phone number. Valid formats are 0XX-XXXXXXXX, composed of 3 or 4 digits of
  region code and 7 or 8 digits of phone number.

* forms.CNCellNumberField: A form field that validates input as a Chinese
  mobile phone number. Valid formats are like 1XXXXXXXXXX, where X is a digit.
  The second digit could only be 3, 5 and 8.

See the source code for full details.

About localflavors
==================

Django's "localflavor" packages offer additional functionality for particular
countries or cultures.

For example, these might include form fields for your country's postal codes,
phone number formats or government ID numbers.

This code used to live in Django proper -- in django.contrib.localflavor -- but
was separated into standalone packages in Django 1.5 to keep the framework's
core clean.

For a full list of available localflavors, see https://github.com/django/
