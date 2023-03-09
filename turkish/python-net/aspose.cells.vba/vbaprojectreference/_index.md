---
title: VbaProjectReference sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 40
url: /tr/python-net/aspose.cells.vba/vbaprojectreference/
is_root: false
---
##  VbaProjectReference sınıfı
VBA projesinin referansını temsil eder.



VbaProjectReference türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [type](/cells/tr/python-net/aspose.cells.vba/vbaprojectreference/type) | Bu başvurunun türünü alır.|
| [name](/cells/tr/python-net/aspose.cells.vba/vbaprojectreference/name) | Başvurunun adını alır ve ayarlar.|
| [libid](/cells/tr/python-net/aspose.cells.vba/vbaprojectreference/libid) | Referansın libidini alır ve ayarlar.|
| [twiddledlibid](/cells/tr/python-net/aspose.cells.vba/vbaprojectreference/twiddledlibid) | Referansın karışık Libid'ini alır ve ayarlar.|
| [extended_libid](/cells/tr/python-net/aspose.cells.vba/vbaprojectreference/extended_libid) | Referansın genişletilmiş Libid'ini alır ve ayarlar.|
| [relative_libid](/cells/tr/python-net/aspose.cells.vba/vbaprojectreference/relative_libid) | Başvurulan VBA projesinin tanımlayıcısını göreli bir yolla alır ve ayarlar.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [copy(source)](/cells/tr/python-net/aspose.cells.vba/vbaprojectreference/copy/#VbaProjectReference) |  |



###  örnekler

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

###  Ayrıca bakınız
* modül [aspose.cells.vba](..)
