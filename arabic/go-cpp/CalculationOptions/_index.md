---
title: "فئة CalculationOptions"
linktitle: "CalculationOptions"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة CalculationOptions. يغلف الكائن الذي يمثل calculationoptions في Go."
type: docs
weight: 200
url: /ar/go-cpp/calculationoptions/
---

## CalculationOptions class

يمثل خيارات الحساب.

```go

type CalculationOptions struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewCalculationOptions](./newcalculationoptions/) | البناء الافتراضي. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetIgnoreError](./getignoreerror/) | يشير إلى ما إذا كان يجب تجاهل الأخطاء التي تم مواجهتها أثناء حساب الصيغ. قد يكون الخطأ دالة غير مدعومة أو روابط خارجية، إلخ. القيمة الافتراضية هي true. |
| [SetIgnoreError](./setignoreerror/) | يشير إلى ما إذا كان يجب تجاهل الأخطاء التي تم مواجهتها أثناء حساب الصيغ. قد يكون الخطأ دالة غير مدعومة أو روابط خارجية، إلخ. القيمة الافتراضية هي true. |
| [GetRecursive](./getrecursive/) | يشير إلى ما إذا كان يتم حساب الخلايا التابعة بشكل متكرر عند حساب خلية واحدة وتعتمد على خلايا أخرى. القيمة الافتراضية هي true. |
| [SetRecursive](./setrecursive/) | يشير إلى ما إذا كان يتم حساب الخلايا التابعة بشكل متكرر عند حساب خلية واحدة وتعتمد على خلايا أخرى. القيمة الافتراضية هي true. |
| [GetUserSpecifiedRefreshDynamicArrayFormula](./getuserspecifiedrefreshdynamicarrayformula/) | يشير إلى ما إذا كان المستخدم قد حدد صراحة سلوك تحديث صيغ المصفوفة الديناميكية قبل حساب الصيغ المحددة. |
| [GetRefreshDynamicArrayFormula](./getrefreshdynamicarrayformula/) | يشير إلى ما إذا كان يجب تحديث صيغ المصفوفة الديناميكية قبل حساب الصيغ. |
| [SetRefreshDynamicArrayFormula](./setrefreshdynamicarrayformula/) | يشير إلى ما إذا كان يجب تحديث صيغ المصفوفة الديناميكية قبل حساب الصيغ. |
| [GetCustomEngine](./getcustomengine/) | محرك حساب الصيغ المخصص لتوسيع محرك الحساب الافتراضي في Aspose.Cells. |
| [SetCustomEngine](./setcustomengine/) | محرك حساب الصيغ المخصص لتوسيع محرك الحساب الافتراضي في Aspose.Cells. |
| [GetCalcStackSize](./getcalcstacksize/) | حجم المكدس لحساب الخلايا بشكل متكرر. القيمة الافتراضية هي 200. |
| [SetCalcStackSize](./setcalcstacksize/) | حجم المكدس لحساب الخلايا بشكل متكرر. القيمة الافتراضية هي 200. |
| [GetPrecisionStrategy](./getprecisionstrategy/) | يحدد الاستراتيجية لمعالجة دقة الحساب. |
| [SetPrecisionStrategy](./setprecisionstrategy/) | يحدد الاستراتيجية لمعالجة دقة الحساب. |
| [GetLinkedDataSources](./getlinkeddatasources/) | يحدد مصادر البيانات للروابط الخارجية المستخدمة في الصيغ. |
| [SetLinkedDataSources](./setlinkeddatasources/) | يحدد مصادر البيانات للروابط الخارجية المستخدمة في الصيغ. |
| [GetCharacterEncoding](./getcharacterencoding/) | يحدد الترميز المستخدم لتشفير/فك تشفير الأحرف عند حساب الصيغ. بالنسبة للدوال مثل CHAR و CODE، تعتمد النتيجة المحسوبة على إعدادات المنطقة ومجموعة الأحرف الافتراضية للبيئة. باستخدام هذه الخاصية يمكن للمستخدم تحديد الترميز المناسب لتلك الدوال للحصول على النتيجة المتوقعة. |
| [SetCharacterEncoding](./setcharacterencoding/) | يحدد الترميز المستخدم لتشفير/فك تشفير الأحرف عند حساب الصيغ. بالنسبة للدوال مثل CHAR و CODE، تعتمد النتيجة المحسوبة على إعدادات المنطقة ومجموعة الأحرف الافتراضية للبيئة. باستخدام هذه الخاصية يمكن للمستخدم تحديد الترميز المناسب لتلك الدوال للحصول على النتيجة المتوقعة. |
