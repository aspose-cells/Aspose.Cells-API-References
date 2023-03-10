---
title: طريقة start_access_cache
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 380
url: /ar/python-net/aspose.cells/workbook/start_access_cache/
is_root: false
---
##  start_access_cache(opts) {#AccessCacheOptions}
يبدأ الجلسة التي تستخدم ذاكرات التخزين المؤقت للوصول إلى البيانات.



```python
def start_access_cache(self, opts):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| opts | [AccessCacheOptions](/cells/ar/python-net/aspose.cells/accesscacheoptions) | خيارات الوصول إلى البيانات|
###  ملاحظات

إذا كانت ذاكرة التخزين المؤقت للوصول إلى البيانات المحددة تتطلب أن تكون بعض نماذج البيانات في ورقة العمل "للقراءة فقط" ،
ثم سيتم اعتبار نماذج البيانات المقابلة في كل ورقة عمل في هذا المصنف على أنها "للقراءة فقط"
ويجب ألا يغير المستخدم أيًا منها.


بعد الانتهاء من الوصول إلى البيانات يجب على [Workbook.close_access_cache(opts)](/cells/ar/python-net/aspose.cells/workbook/close_access_cache)
يتم استدعاؤها بنفس الخيارات لمسح جميع ذاكرات التخزين المؤقت واستعادة وضع الوصول العادي.


###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [Workbook](/cells/ar/python-net/aspose.cells/workbook)
