---
title: طريقة add_identify
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 20
url: /ar/python-net/aspose.cells.pivot/pivotpagefields/add_identify/
is_root: false
---
##  add_identify(range_index, page_item_index) {#int-list}
يعيّن تسمية العنصر في كل حقل صفحة لاستخدامه في تحديد نطاق البيانات.
يجب أن تكون قيمة pageItemIndex.Length مساوية لـ PageFieldCount ، لذا يُرجى إضافة حقل الصفحة أولاً.



```python
def add_identify(self, range_index, page_item_index):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| range_index | int |مؤشر نطاق بيانات التوحيد.|
| page_item_index | list | فهرس عنصر الصفحة في حقل كل صفحة.<br/>pageItemIndex [2] = 1 تعني العنصر الثاني في الحقل الثالث الذي يجب استخدامه لتعريف هذا النطاق.<br/> pageItemIndex [1] = -1 يعني عدم وجود عنصر في الحقل الثاني لاستخدامه لتعريف هذا النطاق<br/> وسيقوم MS تلقائيًا بإنشاء عنصر "فارغ" في الحقل الثاني لتحديد هذا النطاق.|



###  أنظر أيضا
* وحدة [aspose.cells.pivot](../../)
* فئة [PivotPageFields](/cells/ar/python-net/aspose.cells.pivot/pivotpagefields)
