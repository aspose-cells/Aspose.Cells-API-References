---
title: preferred_parsers الملكية
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 300
url: /ar/python-net/aspose.cells/txtloadoptions/preferred_parsers/
is_root: false
---
##  preferred_parsers الملكية

الحصول على وتعيين محللات القيمة المفضلة لتحميل ملف نصي.

###  ملاحظات

المحلل اللغوي [0] هو المحلل اللغوي الذي سيتم استخدامه للعمود الأول في ملف القالب النصي ،
المحلل اللغوي [1] هو المحلل اللغوي الذي سيتم استخدامه للعمود الثاني ، ... إلخ.
سيتم استخدام آخر (parsers [parsers.length-1]) لجميع الأعمدة الأخرى التي تبدأ من parsers.length-1.
إذا كان عنصر واحد فارغًا ، فسيتم تحليل العمود المقابل بواسطة المحلل اللغوي الافتراضي Aspose.Cells.
###  تعريف:
```python
@property
def preferred_parsers(self):
    ...
@preferred_parsers.setter
def preferred_parsers(self, value):
    ...
```

###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [TxtLoadOptions](/cells/ar/python-net/aspose.cells/txtloadoptions)
