---
title: VbaProject sınıf
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 30
url: /tr/python-net/aspose.cells.vba/vbaproject/
is_root: false
---
##  VbaProject sınıf
VBA projesini temsil eder.



VbaProject türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [is_valid_signed](/cells/tr/python-net/aspose.cells.vba/vbaproject/is_valid_signed) | VBA projesi imzasının geçerli olup olmadığını gösterir.|
| [cert_raw_data](/cells/tr/python-net/aspose.cells.vba/vbaproject/cert_raw_data) | Bu VBA projesi imzalanırsa sertifika ham verilerini alır.|
| [name](/cells/tr/python-net/aspose.cells.vba/vbaproject/name) | VBA projesinin adını alır ve ayarlar.|
| [is_signed](/cells/tr/python-net/aspose.cells.vba/vbaproject/is_signed) | VBAcode'un imzalanıp imzalanmadığını gösterir.|
| [is_protected](/cells/tr/python-net/aspose.cells.vba/vbaproject/is_protected) | Bu VBA projesinin korunup korunmadığını gösterir.|
| [islocked_for_viewing](/cells/tr/python-net/aspose.cells.vba/vbaproject/islocked_for_viewing) | Bu VBA projesinin görüntüleme için kilitli olup olmadığını gösterir.|
| [modules](/cells/tr/python-net/aspose.cells.vba/vbaproject/modules) | Tüm [VbaModule](/cells/tr/python-net/aspose.cells.vba/vbamodule) nesnelerini alır.|
| [references](/cells/tr/python-net/aspose.cells.vba/vbaproject/references) | VBA projesinin tüm referanslarını alır.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [sign(digital_signature)](/cells/tr/python-net/aspose.cells.vba/vbaproject/sign/#aspose.cells.digitalsignatures.DigitalSignature) | Bu VBA projesini DigitalSignature ile imzalayın|
| [protect(islocked_for_viewing, password)](/cells/tr/python-net/aspose.cells.vba/vbaproject/protect/#bool-str) | Bu VBA projesini korur veya korumasını kaldırır.|
| [copy(source)](/cells/tr/python-net/aspose.cells.vba/vbaproject/copy/#VbaProject) | Diğer dosyadan VBA projesini kopyalayın.|
| [validate_password(password)](/cells/tr/python-net/aspose.cells.vba/vbaproject/validate_password/#str) | Koruma parolasını doğrular.|



###  Örnek

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Init VBA project.
vbaProject = workbook.vba_project
# Saving the Excel file
workbook.save("book1.xlsm")

```

###  Ayrıca bakınız
* modül [aspose.cells.vba](..)
* sınıf [VbaModule](/cells/tr/python-net/aspose.cells.vba/vbamodule)
