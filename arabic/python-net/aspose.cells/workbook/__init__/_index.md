---
title: Workbook المنشئ
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 10
url: /ar/python-net/aspose.cells/workbook/__init__/
is_root: false
---
##  Workbook() {#}
يقوم بتهيئة نسخة جديدة من الفئة [Workbook](/cells/ar/python-net/aspose.cells/workbook).



```python
def __init__(self):
    ...
```


###  ملاحظات

نوع تنسيق الملف الافتراضي هو Xlsx. لإنشاء نوع ملف بتنسيق آخر ، يرجى استخدام Workbook (FileFormatType).
###  مثال


يوضح الكود التالي كيفية استخدام المُنشئ Workbook لإنشاء مثيل جديد للفئة وتهيئته.

```python
from aspose.cells import Workbook

workbook = Workbook()

```


##  Workbook(file_format_type) {#FileFormatType}
يقوم بتهيئة نسخة جديدة من الفئة [Workbook](/cells/ar/python-net/aspose.cells/workbook).



```python
def __init__(self, file_format_type):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| file_format_type | [FileFormatType](/cells/ar/python-net/aspose.cells/fileformattype) | تنسيق الملف الجديد.|
###  ملاحظات

نوع تنسيق الملف الافتراضي هو Excel97To2003.
###  مثال


يوضح الكود التالي كيفية استخدام المُنشئ Workbook لإنشاء مثيل جديد للفئة وتهيئته.

```python
from aspose.cells import FileFormatType, Workbook

workbook = Workbook(FileFormatType.XLSX)

```


##  Workbook(file) {#str}
يقوم بتهيئة نسخة جديدة من الفئة [Workbook](/cells/ar/python-net/aspose.cells/workbook) وفتح ملف.



```python
def __init__(self, file):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| file | str | اسم الملف.|


##  Workbook(stream) {#io.RawIOBase}
يقوم بتهيئة نسخة جديدة من الفئة [Workbook](/cells/ar/python-net/aspose.cells/workbook) وافتح تدفق.



```python
def __init__(self, stream):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| stream | io.RawIOBase | الدفق.|


##  Workbook(file, load_options) {#str-LoadOptions}
يقوم بتهيئة نسخة جديدة من الفئة [Workbook](/cells/ar/python-net/aspose.cells/workbook) وفتح ملف.



```python
def __init__(self, file, load_options):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| file | str | اسم الملف.|
| load_options | [LoadOptions](/cells/ar/python-net/aspose.cells/loadoptions) | خيارات التحميل|


##  Workbook(stream, load_options) {#io.RawIOBase-LoadOptions}
يقوم بتهيئة نسخة جديدة من الفئة [Workbook](/cells/ar/python-net/aspose.cells/workbook) وفتح الدفق.



```python
def __init__(self, stream, load_options):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| stream | io.RawIOBase | الدفق.|
| load_options | [LoadOptions](/cells/ar/python-net/aspose.cells/loadoptions) | خيارات التحميل|



###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [Workbook](/cells/ar/python-net/aspose.cells/workbook)
