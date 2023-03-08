---
title: طريقة start_cell
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 40
url: /ar/python-net/aspose.cells/lightcellsdatahandler/start_cell/
is_root: false
---
##  start_cell(column_index) {#int}
يستعد لمعالجة الخلية.


###  عائدات

ما إذا كانت هذه الخلية بحاجة إلى المعالجة. خطأ لتجاهل الخلية والتحقق من الخلية التالية حتى تصل إلى نهاية بيانات الخلايا للصف الحالي


```python
def start_cell(self, column_index):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| column_index | int | فهرس العمود للخلية المراد معالجتها|
###  ملاحظات

سيتم استدعاؤه عند الوصول إلى خلية موجودة في الصف الحالي. الصف الحالي هو صف آخر مكالمة [LightCellsDataHandler.process_row(row)](/cells/ar/python-net/aspose.cells/lightcellsdatahandler/process_row).


###  أنظر أيضا

* وحدة [aspose.cells](../../)
* فئة [LightCellsDataHandler](/cells/ar/python-net/aspose.cells/lightcellsdatahandler)
