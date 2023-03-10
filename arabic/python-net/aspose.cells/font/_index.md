---
title: Font الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 650
url: /ar/python-net/aspose.cells/font/
is_root: false
---
##  Font الدرجة
لتغليف كائن الخط المستخدم في جدول بيانات.



يكشف نوع Font الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [charset](/cells/ar/python-net/aspose.cells/font/charset) | تمثيل مجموعة الأحرف.|
| [is_italic](/cells/ar/python-net/aspose.cells/font/is_italic) | الحصول على أو تحديد قيمة تشير إلى ما إذا كان الخط مائلاً.|
| [is_bold](/cells/ar/python-net/aspose.cells/font/is_bold) |الحصول على أو تحديد قيمة تشير إلى ما إذا كان الخط غامقًا أم لا.|
| [caps_type](/cells/ar/python-net/aspose.cells/font/caps_type) | الحصول على نوع الأحرف الاستهلالية للنص وتعيينه.|
| [strike_type](/cells/ar/python-net/aspose.cells/font/strike_type) | يحصل على نوع الإضراب للنص.|
| [is_strikeout](/cells/ar/python-net/aspose.cells/font/is_strikeout) | الحصول على أو تحديد قيمة تشير إلى ما إذا كان الخط عبارة عن خط واحد.|
| [script_offset](/cells/ar/python-net/aspose.cells/font/script_offset) | الحصول على تعويض البرنامج النصي وتعيينه ، في وحدة النسبة المئوية|
| [is_superscript](/cells/ar/python-net/aspose.cells/font/is_superscript) | الحصول على أو تحديد قيمة تشير إلى ما إذا كان الخط نصيًا ممتازًا.|
| [is_subscript](/cells/ar/python-net/aspose.cells/font/is_subscript) | الحصول على أو تحديد قيمة تشير إلى ما إذا كان الخط منخفضًا.|
| [underline](/cells/ar/python-net/aspose.cells/font/underline) | الحصول على نوع تسطير الخط أو تحديده.|
| [name](/cells/ar/python-net/aspose.cells/font/name) | الحصول على أو تحديد اسم [Font](/cells/ar/python-net/aspose.cells/font).|
| [double_size](/cells/ar/python-net/aspose.cells/font/double_size) | الحصول على الحجم المزدوج للخط وتعيينه.|
| [size](/cells/ar/python-net/aspose.cells/font/size) | الحصول على حجم الخط أو تحديده.|
| [theme_color](/cells/ar/python-net/aspose.cells/font/theme_color) | الحصول على لون المظهر وتعيينه.|
| [color](/cells/ar/python-net/aspose.cells/font/color) | الحصول على لون الخط أو تحديده.|
| [argb_color](/cells/ar/python-net/aspose.cells/font/argb_color) | الحصول على اللون وتعيينه بقيمة ARGB 32 بت.|
| [is_normalize_heights](/cells/ar/python-net/aspose.cells/font/is_normalize_heights) | يشير إلى ما إذا كان يتم تطبيق تسوية الارتفاع على تشغيل النص.|
| [scheme_type](/cells/ar/python-net/aspose.cells/font/scheme_type) | الحصول على نوع مخطط الخط وتعيينه.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [equals(font)](/cells/ar/python-net/aspose.cells/font/equals/#Font) | للتحقق مما إذا كان خطان متساويان.|



###  مثال

```python
from aspose.cells import Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[0]
# Accessing the "A1" cell from the worksheet
cell = worksheet.cells.get("A1")
# Adding some value to the "A1" cell
cell.put_value("Hello Aspose!")
font = cell.get_style().font
# Setting the font name to "Times New Roman"
font.name = "Times New Roman"
# Setting font size to 14
font.size = 14
# setting font color as Red
font.color = Color.red
# Saving the Excel file
workbook.save(r"dest.xls")

```

###  أنظر أيضا
* وحدة [aspose.cells](..)
* فئة [Font](/cells/ar/python-net/aspose.cells/font)
