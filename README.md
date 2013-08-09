DNAOrderApp
===========

A web application that aims to improve the interface for ordering DNA sequences from our collaborators in hopes to reduce the error rate of mislabelling wells.

Installation
============
For Mac OSX, first install macports, then:
```bash
# Install prerequisites using macports
port install py27-virtualenv py27-mysql py27-django
# Configure a python virtualenv 
virtualenv-2.7 ~/python-virtualenv
# Enter the virtualenv
. ~/python-virtualenv/bin/activate
# Clone git repository into virtualenv directory and install settings template
(cd ~/python-virtualenv &&  git clone https://github.com/wtsi-hgi/DNAOrderApp.git && cp DNAOrderApp/DNAOrderApp/settings.py.tmpl DNAOrderApp/DNAOrderApp/settings.py)
# Edit settings (DNAOrderApp/DNAOrderApp/settings.py) as needed (with your favorite text editor)
emacs ~/python-virtualenv/DNAOrderApp/DNAOrderApp/settings.py
# Run server
VIRTUAL_ENV=$(echo ~/python-virtualenv) python ~/python-virtualenv/DNAOrderApp/manage.py runserver
```

On Ubuntu Linux, you could run:
```bash
# Install prerequisites
sudo apt-get install python-virtualenv
sudo apt-get build-dep python-mysqldb
# Configure a python virtualenv 
virtualenv ~/python-virtualenv 
# Enter the virtualenv
. ~/python-virtualenv/bin/activate
# Install django and mysqldb
pip install Django
pip install MySQL-python
# Clone git repository into virtualenv directory and install settings template
(cd ~/python-virtualenv &&  git clone https://github.com/wtsi-hgi/DNAOrderApp.git && cp DNAOrderApp/DNAOrderApp/settings.py.tmpl DNAOrderApp/DNAOrderApp/settings.py)
# Edit settings (DNAOrderApp/DNAOrderApp/settings.py) as needed (with your favorite text editor)
emacs ~/python-virtualenv/DNAOrderApp/DNAOrderApp/settings.py
# Run server
python ~/python-virtualenv/DNAOrderApp/manage.py runserver
```

Forked
=======
https://github.com/jschr/bootstrap-modal <br>
https://github.com/sigurdga/django-jquery-file-upload <br>
https://github.com/doph/minimal-django-file-upload-example <br>
https://github.com/python-excel/xlrd <br>

Other JQuery
==============

https://code.google.com/p/jquery-watermark/
https://github.com/tcrosen/twitter-bootstrap-typeahead

Side Note:
================
Currently using Django v1.4. Note that the interface for handling database transactions is different in the latest v1.6.

License
=======
See LICENSE


