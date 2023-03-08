---
title: SignatureLine الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 640
url: /ar/python-net/aspose.cells.drawing/signatureline/
is_root: false
---
##  SignatureLine الدرجة
تمثل خط التوقيع.



يكشف نوع SignatureLine الأعضاء التالية:

###  المنشئون
| البناء| وصف|
| :- | :- |
| [SignatureLine()](/cells/ar/python-net/aspose.cells.drawing/signatureline/__init__/#) | يبني نسخة جديدة من SignatureLine|


###  ملكيات
| ملكية| وصف|
| :- | :- |
| [id](/cells/ar/python-net/aspose.cells.drawing/signatureline/id) | الحصول على أو تعيين معرف لسطر التوقيع هذا.|
| [provider_id](/cells/ar/python-net/aspose.cells.drawing/signatureline/provider_id) | الحصول على معرف موفر التوقيع وتعيينه.|
| [signer](/cells/ar/python-net/aspose.cells.drawing/signatureline/signer) | يحصل على الموقع ويعينه.|
| [title](/cells/ar/python-net/aspose.cells.drawing/signatureline/title) | يحصل على لقب المغني ويحدده.|
| [email](/cells/ar/python-net/aspose.cells.drawing/signatureline/email) |يحصل ويضبط البريد الإلكتروني للمغني.|
| [is_line](/cells/ar/python-net/aspose.cells.drawing/signatureline/is_line) | يشير إلى ما إذا كان سطر توقيع.|
| [allow_comments](/cells/ar/python-net/aspose.cells.drawing/signatureline/allow_comments) | يشير إلى إمكانية إرفاق التعليقات.|
| [show_signed_date](/cells/ar/python-net/aspose.cells.drawing/signatureline/show_signed_date) | يشير إلى ما إذا كان إظهار التاريخ الموقع.|
| [instructions](/cells/ar/python-net/aspose.cells.drawing/signatureline/instructions) | الحصول على النص المعروض للمستخدم في وقت التوقيع وتعيينه.|



###  مثال

```python
from aspose.cells import Workbook
from aspose.cells.drawing import SignatureLine

# Instantiating a Workbook object
workbook = Workbook()
worksheet = workbook.worksheets[0]
# Adding a picture
imgIndex = worksheet.pictures.add(1, 1, "sample.png")
pic = worksheet.pictures[imgIndex]
#  Create signature line object
s = SignatureLine()
s.signer = "Simon Zhao"
s.title = "Development Lead"
s.email = "Simon.Zhao@aspose.com"
#  Assign the signature line object to Picture.SignatureLine property
pic.signature_line = s
# do your business
# Save the excel file.
workbook.save("result.xlsx")

```

###  أنظر أيضا
* وحدة [aspose.cells.drawing](..)
