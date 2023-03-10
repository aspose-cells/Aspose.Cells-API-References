---
title: DigitalSignatureCollection sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 20
url: /tr/python-net/aspose.cells.digitalsignatures/digitalsignaturecollection/
is_root: false
---
##  DigitalSignatureCollection sınıfı
Bir belgeye iliştirilmiş bir dijital imza koleksiyonu sağlar.



DigitalSignatureCollection türü aşağıdaki üyeleri gösterir:

###  İnşaatçılar
| Yapıcı| Tanım|
| :- | :- |
| [DigitalSignatureCollection()](/cells/tr/python-net/aspose.cells.digitalsignatures/digitalsignaturecollection/__init__/#) |DigitalSignatureCollection'ın kurucusu.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [add(digital_signature)](/cells/tr/python-net/aspose.cells.digitalsignatures/digitalsignaturecollection/add/#DigitalSignature) | DigitalSignatureCollection'a bir imza ekleyin.|



###  Örnek

Aşağıdaki örnek, dijital imzanın nasıl doğrulanacağını gösterir.

```python
from aspose.cells import Workbook

# workbook from a signed source file
signedWorkbook = Workbook(r"signedFile.xlsx")
# wb.IsDigitallySigned is true when the workbook is signed already.
print(signedWorkbook.is_digitally_signed)
# get digitalSignature collection from workbook
existingDsc = signedWorkbook.get_digital_signature()
for existingDs in existingDsc:
    print(existingDs.comments)
    print(existingDs.sign_time)
    print(existingDs.is_valid)

```

###  Ayrıca bakınız
* modül [aspose.cells.digitalsignatures](..)
