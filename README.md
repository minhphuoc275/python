# python

1. Install VirtualENV via pip:
```
C:\Windows\system32>pip install virtualenv
Collecting virtualenv
  Downloading virtualenv-20.4.7-py2.py3-none-any.whl (7.2 MB)
     |████████████████████████████████| 7.2 MB 939 kB/s
Collecting six<2,>=1.9.0
  Downloading six-1.16.0-py2.py3-none-any.whl (11 kB)
Collecting filelock<4,>=3.0.0
  Downloading filelock-3.0.12-py3-none-any.whl (7.6 kB)
Collecting appdirs<2,>=1.4.3
  Downloading appdirs-1.4.4-py2.py3-none-any.whl (9.6 kB)
Collecting distlib<1,>=0.3.1
  Downloading distlib-0.3.2-py2.py3-none-any.whl (338 kB)
     |████████████████████████████████| 338 kB 3.3 MB/s
Installing collected packages: six, filelock, distlib, appdirs, virtualenv
Successfully installed appdirs-1.4.4 distlib-0.3.2 filelock-3.0.12 six-1.16.0 virtualenv-20.4.7

C:\Windows\system32>
```
2. Check if Register script folder to Windows Path ENV:
- Go to "C:\Users\<username>\AppData\Local\Programs\Python\Python39\Scripts"

3. Install virtualenvwrapper (https://virtualenvwrapper.readthedocs.io/en/latest/install.html)
```
C:\Windows\system32>pip install virtualenvwrapper-win
Collecting virtualenvwrapper-win
  Downloading virtualenvwrapper-win-1.2.6.tar.gz (21 kB)
Requirement already satisfied: virtualenv in c:\users\phuoctm8\appdata\local\programs\python\python39\lib\site-packages (from virtualenvwrapper-win) (20.4.7)
Requirement already satisfied: six<2,>=1.9.0 in c:\users\phuoctm8\appdata\local\programs\python\python39\lib\site-packages (from virtualenv->virtualenvwrapper-win) (1.16.0)
Requirement already satisfied: distlib<1,>=0.3.1 in c:\users\phuoctm8\appdata\local\programs\python\python39\lib\site-packages (from virtualenv->virtualenvwrapper-win) (0.3.2)
Requirement already satisfied: filelock<4,>=3.0.0 in c:\users\phuoctm8\appdata\local\programs\python\python39\lib\site-packages (from virtualenv->virtualenvwrapper-win) (3.0.12)
Requirement already satisfied: appdirs<2,>=1.4.3 in c:\users\phuoctm8\appdata\local\programs\python\python39\lib\site-packages (from virtualenv->virtualenvwrapper-win) (1.4.4)
Using legacy 'setup.py install' for virtualenvwrapper-win, since package 'wheel' is not installed.
Installing collected packages: virtualenvwrapper-win
    Running setup.py install for virtualenvwrapper-win ... done
Successfully installed virtualenvwrapper-win-1.2.6

C:\Windows\system32>
```

4. Using:
```
C:\Windows\system32>lsvirtualenv

dir /b /ad "C:\Users\phuoctm8\Envs"
==============================================================================
File Not Found

C:\Windows\system32>mkvirtualenv python2104E
 C:\Users\phuoctm8\Envs is not a directory, creating
created virtual environment CPython3.9.5.final.0-64 in 3917ms
  creator CPython3Windows(dest=C:\Users\phuoctm8\Envs\python2104E, clear=False, no_vcs_ignore=False, global=False)
  seeder FromAppData(download=False, pip=bundle, setuptools=bundle, wheel=bundle, via=copy, app_data_dir=C:\Users\phuoctm8\AppData\Local\pypa\virtualenv)
    added seed packages: pip==21.1.2, setuptools==57.0.0, wheel==0.36.2
  activators BashActivator,BatchActivator,FishActivator,PowerShellActivator,PythonActivator,XonshActivator

(python2104E) C:\Windows\System32>lsvirtualenv

dir /b /ad "C:\Users\phuoctm8\Envs"
==============================================================================
python2104E

(python2104E) C:\Windows\System32>mkvirtualenv test01
created virtual environment CPython3.9.5.final.0-64 in 688ms
  creator CPython3Windows(dest=C:\Users\phuoctm8\Envs\test01, clear=False, no_vcs_ignore=False, global=False)
  seeder FromAppData(download=False, pip=bundle, setuptools=bundle, wheel=bundle, via=copy, app_data_dir=C:\Users\phuoctm8\AppData\Local\pypa\virtualenv)
    added seed packages: pip==21.1.2, setuptools==57.0.0, wheel==0.36.2
  activators BashActivator,BatchActivator,FishActivator,PowerShellActivator,PythonActivator,XonshActivator

(test01) C:\Windows\System32>lsvirtualenv

dir /b /ad "C:\Users\phuoctm8\Envs"
==============================================================================
python2104E
test01

(test01) C:\Windows\System32>rmvirtualenv test01

    Deleted C:\Users\phuoctm8\Envs\test01


C:\Windows\System32>lsvirtualenv

dir /b /ad "C:\Users\phuoctm8\Envs"
==============================================================================
python2104E

C:\Windows\System32>
```
