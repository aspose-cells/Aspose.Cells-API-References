---
title: طريقة get_list_value
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 70
url: /ar/python-net/aspose.cells/validation/get_list_value/
is_root: false
---
##  get_list_value(row, column) {#int-int}
احصل على قيمة قائمة التحقق من صحة الخلية المحددة.


###  عائدات

القيمة المطلوب إنتاج قائمة التحقق من الصحة للخلية المحددة.
إذا كانت القائمة تشير إلى نطاق ، فإن القيمة التي تم إرجاعها ستكون عنصر [ReferredArea](/cells/ar/python-net/aspose.cells/referredarea) ؛
وبخلاف ذلك ، قد تكون القيمة التي تم إرجاعها خالية ، أو كائن [] ، أو كائن بسيط.


```python
def get_list_value(self, row, column):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| row | int | فهرس الصف.|
| column | int | فهرس العمود.|
###  ملاحظات

فقط من أجل التحقق من نوع النوع الذي تم تطبيقه على خلية معينة ،
وإلا سيتم إرجاع قيمة خالية.


###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [ReferredArea](/cells/ar/python-net/aspose.cells/referredarea)
* فئة [Validation](/cells/ar/python-net/aspose.cells/validation)
