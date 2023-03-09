---
title: VbaModule sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 10
url: /tr/python-net/aspose.cells.vba/vbamodule/
is_root: false
---
##  VbaModule sınıfı
VBA projesindeki modülü temsil eder.



VbaModule türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [name](/cells/tr/python-net/aspose.cells.vba/vbamodule/name) | Module adını alır ve ayarlar.|
| [type](/cells/tr/python-net/aspose.cells.vba/vbamodule/type) | Modül tipini alır.|
| [codes](/cells/tr/python-net/aspose.cells.vba/vbamodule/codes) | Modüllerin kodlarını alır ve ayarlar.|



###  örnekler

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

###  Ayrıca bakınız
* modül [aspose.cells.vba](..)
