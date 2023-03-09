---
title: VbaModule класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 10
url: /ru/python-net/aspose.cells.vba/vbamodule/
is_root: false
---
##  VbaModule класс
Представляет модуль в проекте VBA.



Тип VbaModule предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [name](/cells/ru/python-net/aspose.cells.vba/vbamodule/name) | Получает и задает имя модуля.|
| [type](/cells/ru/python-net/aspose.cells.vba/vbamodule/type) | Получает тип модуля.|
| [codes](/cells/ru/python-net/aspose.cells.vba/vbamodule/codes) | Получает и устанавливает коды модулей.|



###  Примеры

```python
from aspose.cells import Workbook
from aspose.cells.vba import VbaModuleType

# Instantiating a Workbook object
workbook = Workbook()
#  Init VBA project.
vbaProject = workbook.vba_project
#  Add a new module.
index = vbaProject.modules.add(VbaModuleType.CLASS, "test")
#  Get vba module
vbaModule = vbaProject.modules[index]
#  Set codes
vbaModule.codes = "Sub ShowMessage()\r\nMsgBox \"Welcome to Aspose!\"\r\nEnd Sub"
# Saving the Excel file
workbook.save("book1.xlsm")

```

###  Смотрите также
* модуль [aspose.cells.vba](..)
