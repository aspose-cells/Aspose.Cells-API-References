---
title: classe VbaModule
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 10
url: /it/python-net/aspose.cells.vba/vbamodule/
is_root: false
---
##  classe VbaModule
Rappresenta il modulo nel progetto VBA.



Il tipo VbaModule espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [name](/cells/it/python-net/aspose.cells.vba/vbamodule/name) | Ottiene e imposta il nome di Module.|
| [type](/cells/it/python-net/aspose.cells.vba/vbamodule/type) | Ottiene il tipo di modulo.|
| [codes](/cells/it/python-net/aspose.cells.vba/vbamodule/codes) | Ottiene e imposta i codici dei moduli.|



###  Esempi

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

###  Guarda anche
* modulo [aspose.cells.vba](..)
