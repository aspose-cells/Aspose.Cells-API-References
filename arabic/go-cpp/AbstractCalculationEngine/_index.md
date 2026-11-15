---
title: "فئة AbstractCalculationEngine"
linktitle: "AbstractCalculationEngine"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة AbstractCalculationEngine. تغلف الكائن الذي يمثل abstractcalculationengine في Go."
type: docs
weight: 200
url: /ar/go-cpp/abstractcalculationengine/
---

## AbstractCalculationEngine class

يمثل محرك الحساب المخصص للمستخدم لتوسيع محرك الحساب الافتراضي في Aspose.Cells.

```go

type AbstractCalculationEngine struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |

## طرق

| طريقة | الوصف |
| --- | --- |
| [SkipCalculation](./skipcalculation/) | يتخطى الحساب للمعادلة بالكامل التي تشير إلى الدالة الحالية قيد التقييم. |
| [IsParamLiteralRequired](./isparamliteralrequired/) | يشير إلى ما إذا كان هذا المحرك يحتاج إلى النص الحرفي للمعامل أثناء إجراء الحساب. القيمة الافتراضية هي false. |
| [IsParamArrayModeRequired](./isparamarraymoderequired/) | يشير إلى ما إذا كان هذا المحرك يحتاج إلى حساب المعامل في وضع المصفوفة. القيمة الافتراضية هي false. إذا كان مطلوبًا استدعاء CalculationData.GetParamValueInArrayMode(int, int, int) عند حساب الدوال المخصصة ولم يقم المستخدم بتحديث التعريف لها (عن طريق Workbook.UpdateCustomFunctionDefinition(CustomFunctionDefinition))، يجب ضبط هذه الخاصية إلى true. |
| [GetProcessBuiltInFunctions](./getprocessbuiltinfunctions/) | ما إذا كان يجب فحص ومعالجة الدوال المدمجة التي يدعمها المحرك المدمج بواسطة هذا التنفيذ. القيمة الافتراضية هي false. |
| [ForceRecalculate](./forcerecalculate/) | ما إذا كان يجب إجبار الدالة المعطاة على إعادة حسابها دائمًا عند حساب الصيغ المشتركة. |
