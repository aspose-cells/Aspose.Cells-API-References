---
title: طريقة add
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 20
url: /ar/python-net/aspose.cells/hyperlinkcollection/add/
is_root: false
---
##  add(cell_name, total_rows, total_columns, address) {#str-int-int-str}
يضيف ارتباطًا تشعبيًا إلى خلية محددة أو نطاق من الخلايا.


###  عائدات

[Hyperlink](/cells/ar/python-net/aspose.cells/hyperlink) فهرس العنصر.


```python
def add(self, cell_name, total_rows, total_columns, address):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| cell_name | str | Cell الاسم.|
| total_rows | int | عدد الصفوف في نطاق الارتباط التشعبي هذا.|
| total_columns | int | عدد الأعمدة في نطاق الارتباط التشعبي هذا.|
| address | str | عنوان الارتباط التشعبي.|


##  add(first_row, first_column, total_rows, total_columns, address) {#int-int-int-int-str}
يضيف ارتباطًا تشعبيًا إلى خلية محددة أو نطاق من الخلايا.


###  عائدات

[Hyperlink](/cells/ar/python-net/aspose.cells/hyperlink) فهرس العنصر.


```python
def add(self, first_row, first_column, total_rows, total_columns, address):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| first_row | int | الصف الأول من نطاق الارتباط التشعبي.|
| first_column | int | العمود الأول من نطاق الارتباط التشعبي.|
| total_rows | int | عدد الصفوف في نطاق الارتباط التشعبي هذا.|
| total_columns | int | عدد الأعمدة في نطاق الارتباط التشعبي هذا.|
| address | str | عنوان الارتباط التشعبي.|

###  أمثلة

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
excel = Workbook()
worksheet = excel.worksheets[0]
worksheet.hyperlinks.add("A4", 1, 1, "http://www.aspose.com")
worksheet.hyperlinks.add("A5", 1, 1, "c:\\book1.xls")

```


##  add(start_cell_name, end_cell_name, address, text_to_display, screen_tip) {#str-str-str-str-str}
يضيف ارتباطًا تشعبيًا إلى خلية محددة أو نطاق من الخلايا.


###  عائدات

[Hyperlink](/cells/ar/python-net/aspose.cells/hyperlink) فهرس العنصر.


```python
def add(self, start_cell_name, end_cell_name, address, text_to_display, screen_tip):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| start_cell_name | str | الخلية العلوية اليسرى من النطاق.|
| end_cell_name | str | الخلية اليمنى السفلية من النطاق.|
| address | str | عنوان الارتباط التشعبي.|
| text_to_display | str | النص الذي سيتم عرضه للارتباط التشعبي المحدد.|
| screen_tip | str |نص تلميح الشاشة للارتباط التشعبي المحدد.|



###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [Hyperlink](/cells/ar/python-net/aspose.cells/hyperlink)
* فئة [HyperlinkCollection](/cells/ar/python-net/aspose.cells/hyperlinkcollection)
