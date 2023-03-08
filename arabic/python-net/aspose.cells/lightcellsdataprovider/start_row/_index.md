---
title: طريقة start_row
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 60
url: /ar/python-net/aspose.cells/lightcellsdataprovider/start_row/
is_root: false
---
##  start_row(row) {#Row}
يبدأ في حفظ بيانات صف واحد.



```python
def start_row(self, row):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| row | [Row](/cells/ar/python-net/aspose.cells/row) | كائن الصف للتنفيذ لملء البيانات. فهرس الصف الخاص به هو القيمة التي تم إرجاعها لآخر مكالمة وهي [LightCellsDataProvider.next_row()](/cells/ar/python-net/aspose.cells/lightcellsdataprovider/next_row).<br/>إذا تمت تهيئة الصف في نموذج الخلايا الداخلية ، فسيتم استخدام كائن الصف الموجود.<br/> وإلا فسيتم استخدام كائن صف مؤقت للتنفيذ لملء البيانات.|
###  ملاحظات

سيتم استدعاؤه في بداية حفظ صف وبيانات خلاياه.
إذا كان الصف الحالي يحتوي على بعض الخصائص المخصصة مثل الارتفاع والنمط ... إلخ ،
يجب أن يقوم التنفيذ بتعيين تلك الخصائص على كائن Row المعطى هنا.


###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [LightCellsDataProvider](/cells/ar/python-net/aspose.cells/lightcellsdataprovider)
