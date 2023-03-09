---
title: License класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 980
url: /ru/python-net/aspose.cells/license/
is_root: false
---
##  License класс
Предоставляет методы для лицензирования компонента.



Тип License предоставляет следующие члены:

###  Конструкторы
| Конструктор| Описание|
| :- | :- |
| [License()](/cells/ru/python-net/aspose.cells/license/__init__/#) | Инициализирует новый экземпляр этого класса.|


###  Методы
| Метод| Описание|
| :- | :- |
| [set_license(license_name)](/cells/ru/python-net/aspose.cells/license/set_license/#str) | Лицензирует компоненты.|
| [set_license(stream)](/cells/ru/python-net/aspose.cells/license/set_license/#io.RawIOBase) | Лицензирует компоненты.|



###  Примеры

В этом примере будет предпринята попытка найти файл лицензии с именем MyLicense.lic.
 в папке, содержащей


компонент в папке, содержащей вызывающую сборку,
в папке входной сборки, а затем во встроенных ресурсах вызывающей сборки.

```python
from aspose.cells import License

license = License()
license.set_license("MyLicense.lic")

```

###  Смотрите также
* модуль [aspose.cells](..)
