---
title: classe VbaProjectReference
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 40
url: /it/python-net/aspose.cells.vba/vbaprojectreference/
is_root: false
---
##  classe VbaProjectReference
Rappresenta il riferimento del progetto VBA.



Il tipo VbaProjectReference espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [type](/cells/it/python-net/aspose.cells.vba/vbaprojectreference/type) | Ottiene il tipo di questo riferimento.|
| [name](/cells/it/python-net/aspose.cells.vba/vbaprojectreference/name) | Ottiene e imposta il nome del riferimento.|
| [libid](/cells/it/python-net/aspose.cells.vba/vbaprojectreference/libid) | Ottiene e imposta la Libid del riferimento.|
| [twiddledlibid](/cells/it/python-net/aspose.cells.vba/vbaprojectreference/twiddledlibid) | Ottiene e imposta la Libid modificata del riferimento.|
| [extended_libid](/cells/it/python-net/aspose.cells.vba/vbaprojectreference/extended_libid) | Ottiene e imposta la Libid estesa del riferimento.|
| [relative_libid](/cells/it/python-net/aspose.cells.vba/vbaprojectreference/relative_libid) |Ottiene e imposta l'identificatore del progetto VBA di riferimento con un percorso relativo.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [copy(source)](/cells/it/python-net/aspose.cells.vba/vbaprojectreference/copy/#VbaProjectReference) |  |



###  Esempio

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Init VBA project.
vbaProject = workbook.vba_project
#  Add vba project reference
vbaProject.references.add_registered_reference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation")
# Saving the Excel file
workbook.save("book1.xlsm")

```

###  Guarda anche
* modulo [aspose.cells.vba](..)
