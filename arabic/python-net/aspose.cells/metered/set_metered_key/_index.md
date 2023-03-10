---
title: طريقة set_metered_key
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 40
url: /ar/python-net/aspose.cells/metered/set_metered_key/
is_root: false
---
##  set_metered_key(public_key, private_key) {#str-str}
يضبط المفتاح العام والخاص الذي تم قياسه.
إذا قمت بشراء ترخيص مقنن ، عند بدء التطبيق ، يجب استدعاء هذا API ، عادة ، هذا يكفي. ومع ذلك ، إذا فشلت دائمًا في تحميل بيانات الاستهلاك وتجاوزت 24 ساعة ، فسيتم تعيين الترخيص على حالة التقييم ، لتجنب مثل هذه الحالة ، يجب عليك التحقق بانتظام من حالة الترخيص ، وإذا كانت حالة التقييم ، فاتصل بهذا API مرة أخرى.



```python
def set_metered_key(self, public_key, private_key):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| public_key | str | المفتاح العمومي|
| private_key | str | مفتاح سري|



###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [Metered](/cells/ar/python-net/aspose.cells/metered)
