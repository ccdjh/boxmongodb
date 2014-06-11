![](http://i.v2ex.co/53fQFgQ3.gif) BoxMongodb
==========

----------------------------------------------------------------

boxmongodb is a lightweight ORM framework for Python and MongoDB：

-------------------
#### install (ubuntu)
pip install
``` python
sudo apt-get install mongodb
```
``` python
sudo apt-get install python-pip
```
``` python
sudo pip install boxmongodb
```

-------------------
#### example (ubuntu)

``` python
from boxmongodb import boxmongodb

class mongoMyAnBox_counter(boxmongodb.Model):
    username = boxmongodb.StringProperty()
    num      = boxmongodb.IntegerProperty(default="1")

def main():
        a = "CcdjhMarx"
        b    = "1984"
        m = mongoMyAnBox_counter(username=a,num=b)
        m.insert() 

if __name__ == '__main__':
    main()
```

Documentation
- base 
    - [boxmongodb `*Property` class](#insert)
    - [boxmongodb `Model` function](#insert)
- advanced
    - [creat function ](#insert)
    - [DateTimeProperty ](#insert)


-------------------
####boxmongodb and tornadoWeb
install tornadoWeb
``` python
sudo pip install tornado
``` 
Documentation
- [guide](#insert)
- [boxmongodb guestbook](#insert)
- [boxmongodb Blog](#insert)

-------------------

> download！[click](https://pypi.python.org/pypi/boxmongodb)

-------------------


| author     |    CcdjhMarx(ccdjh.marx@gmail.com) |
| :-------- | :--------:|
| version   | [![Latest Version](http://img.shields.io/pypi/v/boxmongodb.svg)](https://pypi.python.org/pypi/boxmongodb)|
| License  | [![The MIT License](http://img.shields.io/badge/license-MIT-yellow.svg)](https://pypi.python.org/pypi/boxmongodb) |
| install_requires   | Mongodb,pymongo,bson |


-------------------
