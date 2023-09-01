### Clone the repository
* Clone the repository on Windows from the link: https://github.com/shamazkhan/quantlpro

### Initial libraries installation
* Run `pip install -r requirements.txt`
* **Problem:** Install Microsoft C++ Build Tools
* **Solution: From https://visualstudio.microsoft.com/visual-cpp-build-tools/ install tools and use Visual Studio Installer to install the Desktop Tools C++**
* Re run the above mentioned command
* **Problem**: NumPy 1.19.5 may not yet support Python 3.11.
* Now I am trying to switch to python 3.6
* Go to this link and find the desired version https://www.python.org/downloads/windows/
* Download the file where it shows "Windows x86 64-bit executable installer"
* Add python to the PATH variable "C:\Users\Khadija Kamran\AppData\Local\Programs\Python\Python36"
* **Solution: Switch to Python 3.6**
* **Problem**: Command "python setup.py egg_info" failed with error code 1 in C:\Users\KHADIJ~1\AppData\Local\Temp\pip-install-vu1vrpnh\PyQt5\
* The error message you're seeing suggests that there is an issue with the installation of PyQt5, and it's failing during the execution of the command python setup.py egg_info. This error typically occurs when the required build dependencies for PyQt5 are not installed or when there is an issue with the installation process.
* **Solution: upgraded the pip version**
* Setup completed. All the requirements for the libraries are satisfied.
![image](https://github.com/KhadijaKamran/Work-Documentation/assets/46638501/0f9a70c7-ff00-48a3-80d9-ee68a6dde28c)

### Database 
* Run `python manage.py makemigrations`
* Run `python manage.py migrate`

### Runserver
* Run `python manage.py runserver`
* **Problem**: Invalid HTTP_HOST header: '127.0.0.1:8000'. You may need to add '127.0.0.1' to ALLOWED_HOSTS.
* **Solution: Added IP '127.0.0.1' to the ALLOWED_HOSTS dictionary**
```
ALLOWED_HOSTS = ["127.0.0.1","localhost"]
```
* The server runs successfully

### git status
```
modified:   db.sqlite3
modified:   quantlpro/settings.py
```
