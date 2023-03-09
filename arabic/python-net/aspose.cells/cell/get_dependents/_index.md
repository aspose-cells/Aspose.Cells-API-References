---
title: طريقة get_dependents
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 90
url: /ar/python-net/aspose.cells/cell/get_dependents/
is_root: false
---
##  get_dependents(is_all) {#bool}
احصل على جميع الخلايا التي تشير صيغتها إلى هذه الخلية مباشرةً.



```python
def get_dependents(self, is_all):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| is_all | bool | يشير إلى ما إذا كان التحقق من الصيغ في أوراق العمل الأخرى|
###  ملاحظات

* إذا ظهر مرجع واحد يحتوي على هذه الخلية في صيغة خلية واحدة ، فسيتم اعتبار هذه الخلية على أنها

تابع هذه الخلية ، بغض النظر عن المرجع أو هذه الخلية مستخدمة أم لا أثناء الحساب.
على سبيل المثال ، على الرغم من عدم استخدام الخلية A2 في الصيغة "= IF (TRUE، A1، A2)" أثناء الحساب ،
لا تزال هذه الصيغة تؤخذ على أنها تابعة لـ A2.
للحصول على تلك الصيغ التي تعتمد نتائجها المحسوبة على هذه الخلية ، يرجى استخدام [Cell.get_dependents_in_calculation(recursive)](/cells/ar/python-net/aspose.cells/cell/get_dependents_in_calculation). عند تتبع المعالين لخلية واحدة ، سيتم تحليل جميع الصيغ الموجودة في المصنف أو ورقة العمل والتحقق منها.
لذا فهي عملية تستغرق وقتًا طويلاً ، فإذا احتاج المستخدم إلى تتبع المعالين للعديد من الخلايا ، فإن استخدام هذه الطريقة سيفعل
يؤدي إلى أداء ضعيف. للنظر في الأداء ، يجب على المستخدم استخدام [Cell.get_dependents_in_calculation(recursive)](/cells/ar/python-net/aspose.cells/cell/get_dependents_in_calculation) بدلاً من ذلك.
أو ، يمكن للمستخدم جمع خريطة السوابق لجميع الخلايا بواسطة [Cell.get_precedents()](/cells/ar/python-net/aspose.cells/cell/get_precedents) أولاً ،
ثم قم ببناء خريطة المعالين وفقًا لخريطة السوابق.

* إذا ظهر مرجع واحد يحتوي على هذه الخلية في صيغة خلية واحدة ، فسيتم اعتبار هذه الخلية على أنها
تابع هذه الخلية ، بغض النظر عن المرجع أو هذه الخلية مستخدمة أم لا أثناء الحساب.
على سبيل المثال ، على الرغم من عدم استخدام الخلية A2 في الصيغة "= IF (TRUE، A1، A2)" أثناء الحساب ،
لا تزال هذه الصيغة تؤخذ على أنها تابعة لـ A2.
للحصول على تلك الصيغ التي تعتمد نتائجها المحسوبة على هذه الخلية ، يرجى استخدام [Cell.get_dependents_in_calculation(recursive)](/cells/ar/python-net/aspose.cells/cell/get_dependents_in_calculation). عند تتبع المعالين لخلية واحدة ، سيتم تحليل جميع الصيغ الموجودة في المصنف أو ورقة العمل والتحقق منها.
لذا فهي عملية تستغرق وقتًا طويلاً ، فإذا احتاج المستخدم إلى تتبع المعالين للعديد من الخلايا ، فإن استخدام هذه الطريقة سيفعل
يؤدي إلى أداء ضعيف. للنظر في الأداء ، يجب على المستخدم استخدام [Cell.get_dependents_in_calculation(recursive)](/cells/ar/python-net/aspose.cells/cell/get_dependents_in_calculation) بدلاً من ذلك.
أو ، يمكن للمستخدم جمع خريطة السوابق لجميع الخلايا بواسطة [Cell.get_precedents()](/cells/ar/python-net/aspose.cells/cell/get_precedents) أولاً ،
ثم قم ببناء خريطة المعالين وفقًا لخريطة السوابق.

* إذا ظهر مرجع واحد يحتوي على هذه الخلية في صيغة خلية واحدة ، فسيتم اعتبار هذه الخلية على أنها
تابع هذه الخلية ، بغض النظر عن المرجع أو هذه الخلية مستخدمة أم لا أثناء الحساب.
على سبيل المثال ، على الرغم من عدم استخدام الخلية A2 في الصيغة "= IF (TRUE، A1، A2)" أثناء الحساب ،
لا تزال هذه الصيغة تؤخذ على أنها تابعة لـ A2.
للحصول على تلك الصيغ التي تعتمد نتائجها المحسوبة على هذه الخلية ، يرجى استخدام [Cell.get_dependents_in_calculation(recursive)](/cells/ar/python-net/aspose.cells/cell/get_dependents_in_calculation). عند تتبع المعالين لخلية واحدة ، سيتم تحليل جميع الصيغ الموجودة في المصنف أو ورقة العمل والتحقق منها.
لذا فهي عملية تستغرق وقتًا طويلاً ، فإذا احتاج المستخدم إلى تتبع المعالين للعديد من الخلايا ، فإن استخدام هذه الطريقة سيفعل
يؤدي إلى أداء ضعيف. للنظر في الأداء ، يجب على المستخدم استخدام [Cell.get_dependents_in_calculation(recursive)](/cells/ar/python-net/aspose.cells/cell/get_dependents_in_calculation) بدلاً من ذلك.
أو ، يمكن للمستخدم جمع خريطة السوابق لجميع الخلايا بواسطة [Cell.get_precedents()](/cells/ar/python-net/aspose.cells/cell/get_precedents) أولاً ،
ثم قم ببناء خريطة المعالين وفقًا لخريطة السوابق.
###  أمثلة

```python
from aspose.cells import Workbook

workbook = Workbook()
cells = workbook.worksheets[0].cells
cells.get("A1").formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2"
cells.get("A2").formula = "=IF(TRUE,B2,B1)"
dependents = cells.get("B1").get_dependents(True)
for i in range(len(dependents)):
    print(dependents[i].name)

```



###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [Cell](/cells/ar/python-net/aspose.cells/cell)
