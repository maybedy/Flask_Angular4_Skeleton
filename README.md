Flask/Angular 4 - Skeleton
=========================

One thing to note is that flask calls Angular's index.html file located 'static/src/index.html' which serves
the angular app. It is important to note that flask finds the index.html upon building in the 'dist' directory.

Another note is that an efficient way to develop the angular flask app is to use two different terminals.
One terminal will run the server side. (to run server side: python manage.py runserver)
The second terminal will run the client side. (ng build --dev --watch)

============
Requirements
============

- python 3
- pip
- nvm (node version manager)
- npm > 3
- node > 5
- angular cli
- virtualenv

Install Python 3:

    - https://www.python.org/downloads/
    - python -v ( > 3.4 )

Install pip (MAC):

    - sudo easy_install pip

Install pip (WINDOWS):

    - python -m pip install --upgrade pip

Install nvm (MAC):

    - curl https://raw.githubusercontent.com/creationix/nvm/v0.25.0/install.sh | bash
    - close terminal and reopen
    - nvm --version

Install nvm (WINDOWS):

    - https://github.com/coreybutler/nvm-windows/releases
    - close terminal and reopen
    - nvm --version

Install node and npm (with nvm):

    - nvm install 6
    - npm -v
    - node -v

Install Angular CLI:

    - npm install -g @angular/cli
    - ng -v

Install virtualenv:

    - pip install virtualenv

============
Setup
============

1. open terminal
2. cd desktop
3. git clone https://github.com/hawzie197/Flask_Angular4_Skeleton.git
4. cd into Flask_Angular4_Skeleton
5. run create virtual env (see below for mac vs windows)
6. pip install -r requirements.txt
7. python manage.py runserver
8. open second terminal
9. cd app/static
10. check node/npm versions (if not correct, run: nvm use 6) # import because of angular's package-lock.json
11. npm install (get node_modules, could take a while)
12. ng build --dev --watch
13. navigate to: http://127.0.0.1:5000/

VIRTUALENV MAC:

    - virtualenv env
    - source env/bin/activate

VIRTUALENV WINDOWS:

    - virtualenv env
    - cd env/Scripts
    - activate
