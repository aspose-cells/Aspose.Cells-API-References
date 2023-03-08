---
title: DigitalSignatureCollection الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 20
url: /ar/python-net/aspose.cells.digitalsignatures/digitalsignaturecollection/
is_root: false
---
##  DigitalSignatureCollection الدرجة
يوفر مجموعة من التواقيع الرقمية المرفقة بمستند.



يكشف نوع DigitalSignatureCollection الأعضاء التالية:

###  المنشئون
| البناء| وصف|
| :- | :- |
| [DigitalSignatureCollection()](/cells/ar/python-net/aspose.cells.digitalsignatures/digitalsignaturecollection/__init__/#) | مُنشئ DigitalSignatureCollection.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [add(digital_signature)](/cells/ar/python-net/aspose.cells.digitalsignatures/digitalsignaturecollection/add/#DigitalSignature) |أضف توقيعًا واحدًا إلى DigitalSignatureCollection.|



###  مثال

يوضح المثال التالي كيفية التحقق من صحة التوقيع الرقمي.

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

###  أنظر أيضا
* وحدة [aspose.cells.digitalsignatures](..)
