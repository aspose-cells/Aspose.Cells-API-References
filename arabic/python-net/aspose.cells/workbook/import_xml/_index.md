---
title: طريقة import_xml
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 220
url: /ar/python-net/aspose.cells/workbook/import_xml/
is_root: false
---
##  import_xml(url, sheet_name, row, col) {#str-str-int-int}
يستورد / يحدّث ملف بيانات XML في المصنف.



```python
def import_xml(self, url, sheet_name, row, col):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| url | str | عنوان url / مسار ملف xml.|
| sheet_name | str | اسم الورقة الوجهة.|
| row | int | صف الوجهة|
| col | int | عمود الوجهة|

###  مثال

يستورد الكود التالي بيانات xml في ورقة العمل 'Sheet 1' على Cell A1.

```python
from aspose.cells import Workbook

wb = Workbook("Book1.xlsx")
wb.import_xml("xml.xml", "Sheet1", 0, 0)
wb.save("output.xlsx")

```


##  import_xml(stream, sheet_name, row, col) {#io.RawIOBase-str-int-int}
يستورد / يحدّث ملف بيانات XML في المصنف.



```python
def import_xml(self, stream, sheet_name, row, col):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| stream | io.RawIOBase | دفق ملف xml.|
| sheet_name | str | اسم الورقة الوجهة.|
| row | int | صف الوجهة.|
| col | int |عمود الوجهة.|



###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [Workbook](/cells/ar/python-net/aspose.cells/workbook)
