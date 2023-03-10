---
title: طريقة freeze_panes
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 120
url: /ar/python-net/aspose.cells/worksheet/freeze_panes/
is_root: false
---
##  freeze_panes(cell_name, freezed_rows, freezed_columns) {#str-int-int}
تجميد الأجزاء في الخلية المحددة في ورقة العمل.



```python
def freeze_panes(self, cell_name, freezed_rows, freezed_columns):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| cell_name | str | Cell الاسم.|
| freezed_rows | int | عدد الصفوف المرئية في الجزء العلوي ، ليس أكثر من فهرس الصف.|
| freezed_columns | int | عدد الأعمدة المرئية في الجزء الأيمن ، ليس أكثر من فهرس العمود.|
###  ملاحظات

لا يمكن أن يكون فهرس الصف وفهرس العمود صفرًا. عدد الصفوف وعدد الأعمدة
أيضا لا يمكن أن تكون كلها صفرا.

##  freeze_panes(row, column, freezed_rows, freezed_columns) {#int-int-int-int}
تجميد الأجزاء في الخلية المحددة في ورقة العمل.



```python
def freeze_panes(self, row, column, freezed_rows, freezed_columns):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| row | int | فهرس الصف.|
| column | int | فهرس العمود.|
| freezed_rows | int | عدد الصفوف المرئية في الجزء العلوي ، ليس أكثر من فهرس الصف.|
| freezed_columns | int | عدد الأعمدة المرئية في الجزء الأيمن ، ليس أكثر من فهرس العمود.|
###  ملاحظات

لا يمكن أن يكون فهرس الصف وفهرس العمود صفرًا. عدد الصفوف وعدد الأعمدة
أيضا لا يمكن أن تكون كلها صفرا.


تحدد المعلمتان الأوليان موضع التجميد وتحدد المعلمتان الأخيرتان المنطقة المجمدة في الجزء العلوي الأيسر.


###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [Worksheet](/cells/ar/python-net/aspose.cells/worksheet)
