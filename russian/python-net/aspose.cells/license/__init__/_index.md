---
title: License конструктор
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 10
url: /ru/python-net/aspose.cells/license/__init__/
is_root: false
---
##  License() {#}
Инициализирует новый экземпляр этого класса.



```python
def __init__(self):
    ...
```



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
* модуль [aspose.cells](../../)
* класс [License](/cells/ru/python-net/aspose.cells/license)
