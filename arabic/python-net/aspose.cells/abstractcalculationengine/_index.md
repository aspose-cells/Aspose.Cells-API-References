---
title: AbstractCalculationEngine الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 20
url: /ar/python-net/aspose.cells/abstractcalculationengine/
is_root: false
---
##  AbstractCalculationEngine الدرجة
يمثل محرك الحساب المخصص للمستخدم لتوسيع محرك الحساب الافتراضي لـ Aspose.Cells.



يكشف نوع AbstractCalculationEngine الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [is_param_literal_required](/cells/ar/python-net/aspose.cells/abstractcalculationengine/is_param_literal_required) | يشير إلى ما إذا كان هذا المحرك يحتاج إلى النص الحرفي للمعلمة أثناء إجراء الحساب. القيمة الافتراضية هي خطأ.|
| [process_built_in_functions](/cells/ar/python-net/aspose.cells/abstractcalculationengine/process_built_in_functions) | ما إذا كان يجب فحص ومعالجة الوظائف المضمنة التي تم دعمها بواسطة المحرك المدمج من خلال هذا التنفيذ.<br/>الافتراضي هو خطأ.<br/> إذا احتاج المستخدم إلى تغيير منطق الحساب لبعض الوظائف المضمنة ، فيجب تعيين هذه الخاصية على أنها صحيحة.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [calculate(data)](/cells/ar/python-net/aspose.cells/abstractcalculationengine/calculate/#CalculationData) | تحسب دالة واحدة ببيانات معينة.|



###  ملاحظات

يجب ألا يقوم المستخدم بتعديل أي جزء من المصنف مباشرةً في هذا التنفيذ (باستثناء النتيجة المحسوبة للدالة المخصصة ، والتي يمكن تعيينها بواسطة الخاصية CalculationData.CalculatedValue).
خلاف ذلك قد يكون سبب نتيجة غير متوقعة أو استثناء.
إذا احتاج المستخدم إلى تغيير بيانات أخرى غير النتيجة المحسوبة في تنفيذ بعض الوظائف المخصصة ،
على سبيل المثال ، تغيير صيغة الخلية ، النمط ، ... إلخ ، يجب على المستخدم جمع هذه البيانات في هذا التطبيق وتغييرها خارج نطاق حساب الصيغة.

###  أنظر أيضا
* وحدة [aspose.cells](..)
