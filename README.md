![](http://i.v2ex.co/53fQFgQ3.gif) BoxMongodb
==========

----------------------------------------------------------------

boxmongodb is a lightweight ORM framework for Python and MongoDB：

-------------------

> 中文文档 [click](https://github.com/ccdjh/boxmongodb/wiki/ChineseREADME)


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

>*Property class  `StringProperty` ，`DateTimeProperty` ，`IntegerProperty` ，`LinkProperty` ，`AuthProperty` ，`DictProperty` ，`EmailProperty` 

---------------------------------------------------------------

>function：`insert` ， `update` ， `update_id`

>@classmethod：`find`,`find_all`,`find_id`,`insert_dict`,`remove`,`remove_all`,`update_id_dict`


--------------------------------------------------------

Documentation
- base 
    - [boxmongodb `*Property` class](https://github.com/ccdjh/boxmongodb/wiki/EnglishModel)
    - [boxmongodb `Model` function](https://github.com/ccdjh/boxmongodb/wiki/EnglishDef)
- [Advanced documentation](https://github.com/ccdjh/boxmongodb/wiki/EnglishAdvanced#advanced-documentation)
    - [creat function](https://github.com/ccdjh/boxmongodb/wiki/EnglishAdvanced#creat-function)
    - [DateTimeProperty](https://github.com/ccdjh/boxmongodb/wiki/EnglishAdvanced#datetimeproperty)
    - [BoxMongodb connection](https://github.com/ccdjh/boxmongodb/wiki/EnglishAdvanced#boxmongodb-connection)


-------------------
####boxmongodb and tornadoWeb
install tornadoWeb
``` python
sudo pip install tornado
``` 
Documentation
- [boxmongodb guestbook](https://github.com/ccdjh/boxmongodb/wiki/EnglishGuestbook)

-------------------
