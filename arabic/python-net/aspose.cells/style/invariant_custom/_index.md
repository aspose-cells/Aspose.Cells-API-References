---
title: invariant_custom الملكية
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 260
url: /ar/python-net/aspose.cells/style/invariant_custom/
is_root: false
---
##  invariant_custom الملكية

يحصل على سلسلة نمط الثقافة المستقلة لتنسيق الأرقام.
إذا لم يتم تعيين تنسيق رقمي لهذا الكائن ، فسيتم إرجاع قيمة خالية.
إذا كان تنسيق الأرقام مدمجًا ، فسيتم إرجاع سلسلة النمط المقابلة للرقم المضمن.

###  ملاحظات

بالنسبة إلى تنسيقات الأرقام المضمنة ، لا يزال محتوى النمط الذي يتم إرجاعه معتمدًا على الثقافة ،
على سبيل المثال ، بالنسبة لبعض اللغات ، تقوم بإرجاع "m / d / y" وبالنسبة لبعض اللغات الأخرى فإنها ترجع "d / m / y".
الفرق عن [Style.culture_custom](/cells/ar/python-net/aspose.cells/style#culture_custom) هو (هذا أيضًا ما يعنيه الاستقلال الثقافي):
يتم الاحتفاظ بمحددات التنسيق والفواصل بشكل قياسي ، مثل "/" ستستخدم دائمًا كفاصل تاريخ / وقت
سيتم استخدام "y" دائمًا كجزء "السنة" بغض النظر عن الحرف الخاص الآخر المستخدم للإعداد المحلي المحدد.
###  تعريف:
```python
@property
def invariant_custom(self):
    ...
```

###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [Style](/cells/ar/python-net/aspose.cells/style)
