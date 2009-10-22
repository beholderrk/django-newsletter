django-newsletter
=================
Django app for managing multiple mass-mailing lists with both plaintext as well as HTML templates (and TinyMCE editor for HTML messages), images and a smart queueing system all right from the admin interface.

Status
------
We are currently nearing the end of a migration from an early production version to a Django 1.1-compatible release. Might still be a bit buggy though.

Requirements
------------
* Django 1.1
* django-extensions (included in demo app)

Installation
------------
* ``git clone git://github.com/dokterbob/django-newsletter.git``
* ``ln -s django-newsletter/newsletter``
* ``ln -s django-newsletter/media static/newsletter``
* Add newsletter to ``INSTALLED_APPS`` in ``settings.py``
* Run unit tests just to be sure it is working.

Usage
-----
* Start the development server: ``./manage.py runserver``
* Navigate to ``/admin/`` and: behold!
* Put a submission in the queue.
* Make sure django_extensions is installed and:
  ``./manage.py runjob submit``
* For a proper understanding, please take a look at the model graph in .. image:: model_graph.png



TODO
-----
* Connect subcribers to Django auth app User model.