---
title: VbaProjectReference klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 40
url: /sv/python-net/aspose.cells.vba/vbaprojectreference/
is_root: false
---
##  VbaProjectReference klass
Representerar referensen för VBA-projektet.



Typen VbaProjectReference avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [type](/cells/sv/python-net/aspose.cells.vba/vbaprojectreference/type) | Får typen av denna referens.|
| [name](/cells/sv/python-net/aspose.cells.vba/vbaprojectreference/name) | Hämtar och ställer in namnet på referensen.|
| [libid](/cells/sv/python-net/aspose.cells.vba/vbaprojectreference/libid) | Hämtar och ställer in referensens libid.|
| [twiddledlibid](/cells/sv/python-net/aspose.cells.vba/vbaprojectreference/twiddledlibid) | Får och ställer in referensens vridna Libid.|
| [extended_libid](/cells/sv/python-net/aspose.cells.vba/vbaprojectreference/extended_libid) | Hämtar och ställer in referensens utökade Libid.|
| [relative_libid](/cells/sv/python-net/aspose.cells.vba/vbaprojectreference/relative_libid) | Hämtar och ställer in det refererade VBA-projektets identifierare med en relativ sökväg.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [copy(source)](/cells/sv/python-net/aspose.cells.vba/vbaprojectreference/copy/#VbaProjectReference) |  |



###  Exempel

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

###  Se även
* modul [aspose.cells.vba](..)
