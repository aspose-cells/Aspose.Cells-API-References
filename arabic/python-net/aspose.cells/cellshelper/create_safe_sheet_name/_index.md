---
title: طريقة create_safe_sheet_name
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 90
url: /ar/python-net/aspose.cells/cellshelper/create_safe_sheet_name/
is_root: false
---
##  create_safe_sheet_name(name_proposal) {#str}
للتحقق من اسم الورقة المحدد وإنشاء اسم صالح عند الحاجة.
إذا كان اسم الورقة المعطى يتوافق مع قواعد اسم ورقة Excel ، فقم بإعادتها.
وإلا سيتم قطع السلسلة إذا تجاوز الطول الحد
وسيتم استبدال الأحرف غير الصالحة بـ "" ، ثم يتم إرجاع قيمة السلسلة المعاد بناؤها.


###  عائدات




```python
def create_safe_sheet_name(self, name_proposal):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| name_proposal | str | اسم الورقة المطلوب استخدامه|


##  create_safe_sheet_name(name_proposal, replace_char) {#str-char}
للتحقق من اسم الورقة المحدد وإنشاء اسم صالح عند الحاجة.
إذا كان اسم الورقة المعطى يتوافق مع قواعد اسم ورقة Excel ، فقم بإعادتها.
وإلا سيتم قطع السلسلة إذا تجاوز الطول الحد
وسيتم استبدال الأحرف غير الصالحة بحرف معين ، ثم إرجاع قيمة السلسلة المعاد بناؤها.


###  عائدات




```python
def create_safe_sheet_name(self, name_proposal, replace_char):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| name_proposal | str | اسم الورقة المطلوب استخدامه|
| replace_char | char | الحرف الذي سيتم استخدامه لاستبدال الأحرف غير الصالحة في اسم الورقة المحدد|



###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [CellsHelper](/cells/ar/python-net/aspose.cells/cellshelper)
