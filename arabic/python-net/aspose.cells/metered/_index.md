---
title: Metered الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 1050
url: /ar/python-net/aspose.cells/metered/
is_root: false
---
##  Metered الدرجة
يوفر طرقًا لضبط المفاتيح المقننة.



يكشف نوع Metered الأعضاء التالية:

###  المنشئون
| البناء| وصف|
| :- | :- |
| [Metered()](/cells/ar/python-net/aspose.cells/metered/__init__/#) | تهيئة مثيل جديد من هذه الفئة.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [set_metered_key(public_key, private_key)](/cells/ar/python-net/aspose.cells/metered/set_metered_key/#str-str) | يضبط المفاتيح العامة والخاصة المقننة.<br/>إذا قمت بشراء ترخيص مقنن ، عند بدء التطبيق ، يجب استدعاء API ، عادةً ، هذا يكفي.يجب عليك التحقق بانتظام من حالة الترخيص ، إذا كانت حالة التقييم ، فاتصل بهذا API مرة أخرى.|
| [get_consumption_quantity()](/cells/ar/python-net/aspose.cells/metered/get_consumption_quantity/#) | يحصل على حجم ملف الاستهلاك|
| [get_consumption_credit()](/cells/ar/python-net/aspose.cells/metered/get_consumption_credit/#) | يحصل على الائتمان الاستهلاكي|



###  أمثلة

في هذا المثال ، ستُبذل محاولة لتعيين المفاتيح العامة والخاصة التي تم قياسها


```python
from aspose.cells import Metered

matered = Metered()
matered.set_metered_key("PublicKey", "PrivateKey")

```

###  أنظر أيضا
* وحدة [aspose.cells](..)
