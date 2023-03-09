---
title: protect метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 180
url: /ru/python-net/aspose.cells/worksheet/protect/
is_root: false
---
##  protect(type) {#ProtectionType}
Защищает рабочий лист.



```python
def protect(self, type):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| type | [ProtectionType](/cells/ru/python-net/aspose.cells/protectiontype) | Тип защиты.|
###  Примечания

Этот метод защищает рабочий лист без пароля. Он может protect рабочий лист во всех версиях файла Excel.

##  protect(type, password, old_password) {#ProtectionType-str-str}

Защищает рабочий лист.



```python
def protect(self, type, password, old_password):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| type | [ProtectionType](/cells/ru/python-net/aspose.cells/protectiontype) | Тип защиты.|
| password | str | Пароль.|
| old_password | str | Если рабочий лист уже защищен паролем, укажите старый пароль.<br/> В противном случае вы можете установить для этого параметра нулевое значение или пустую строку.|
###  Примечания

Этот метод может работать с рабочим листом protect во всех версиях файла Excel.
###  Пример


```python
from aspose.cells import ProtectionType, Workbook

# Instantiating a Workbook object
excel = Workbook("template.xlsx")
# Accessing the first worksheet in the Excel file
worksheet = excel.worksheets[0]
# Protecting the worksheet with a password
worksheet.protect(ProtectionType.ALL, "aspose", None)
# Saving the modified Excel file in default (that is Excel 20003) format
excel.save("output.xls")

```



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Worksheet](/cells/ru/python-net/aspose.cells/worksheet)
