---
title: طريقة start_sheet
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 70
url: /ar/python-net/aspose.cells/lightcellsdataprovider/start_sheet/
is_root: false
---
##  start_sheet(sheet_index) {#int}
يبدأ في حفظ ورقة العمل.


###  عائدات

صواب إذا كان هذا الموفر سيوفر بيانات للورقة المحددة ؛ خطأ إذا كان يجب أن تستخدم ورقة معينة نموذج البيانات العادي الخاص بها (Cells).


```python
def start_sheet(self, sheet_index):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| sheet_index | int | سيتم حفظ فهرس الورقة الحالية.|
###  ملاحظات

سيتم استدعاؤه في بداية حفظ ورقة العمل أثناء حفظ المصنف.
 إذا كان المزود يحتاج إلى الرجوع إلى*"فهرس الورقة"* لاحقاً
في طريقة startRow (Row) أو startCell (Cell) ،
 أي إذا كانت العملية تحتاج إلى معرفة ورقة العمل التي تتم معالجتها ،
 يجب أن يحتفظ التنفيذ ب*"فهرس الورقة"* القيمة هنا.


###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [LightCellsDataProvider](/cells/ar/python-net/aspose.cells/lightcellsdataprovider)
