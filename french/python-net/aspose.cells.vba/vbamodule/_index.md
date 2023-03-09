---
title: VbaModule classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 10
url: /fr/python-net/aspose.cells.vba/vbamodule/
is_root: false
---
##  VbaModule classe
Représente le module dans le projet VBA.



Le type VbaModule expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [name](/cells/fr/python-net/aspose.cells.vba/vbamodule/name) | Obtient et définit le nom de Module.|
| [type](/cells/fr/python-net/aspose.cells.vba/vbamodule/type) | Obtient le type de module.|
| [codes](/cells/fr/python-net/aspose.cells.vba/vbamodule/codes) | Obtient et définit les codes du module.|



###  Exemple

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

###  Voir également
* module [aspose.cells.vba](..)
