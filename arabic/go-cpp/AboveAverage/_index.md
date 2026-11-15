---
title: "فئة AboveAverage"
linktitle: "AboveAverage"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة AboveAverage. تغلف الكائن الذي يمثل aboveaverage في Go."
type: docs
weight: 200
url: /ar/go-cpp/aboveaverage/
---

## AboveAverage class

صف قاعدة التنسيق الشرطي AboveAverage. تُبرز هذه القاعدة الخلايا التي تكون أعلى أو أقل من المتوسط لجميع القيم في النطاق.

```go

type AboveAverage struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewAboveAverage](./newaboveaverage/) | البناء الافتراضي. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [IsAboveAverage](./isaboveaverage/) | احصل أو عيّن العلامة التي تشير إلى ما إذا كانت القاعدة هي قاعدة \"أعلى من المتوسط\". 'true' يعني 'أعلى من المتوسط'. القيمة الافتراضية هي true. |
| [SetIsAboveAverage](./setisaboveaverage/) | احصل أو عيّن العلامة التي تشير إلى ما إذا كانت القاعدة هي قاعدة \"أعلى من المتوسط\". 'true' يعني 'أعلى من المتوسط'. القيمة الافتراضية هي true. |
| [IsEqualAverage](./isequalaverage/) | احصل أو عيّن العلامة التي تشير إلى ما إذا كانت معايير 'aboveAverage' و 'belowAverage' تشمل المتوسط نفسه أم لا. 'true' يعني تضمين قيمة المتوسط في المعايير. القيمة الافتراضية هي false. |
| [SetIsEqualAverage](./setisequalaverage/) | احصل أو عيّن العلامة التي تشير إلى ما إذا كانت معايير 'aboveAverage' و 'belowAverage' تشمل المتوسط نفسه أم لا. 'true' يعني تضمين قيمة المتوسط في المعايير. القيمة الافتراضية هي false. |
| [GetStdDev](./getstddev/) | احصل أو عيّن عدد الانحرافات المعيارية لتضمينها فوق أو تحت المتوسط في قاعدة التنسيق الشرطي. يجب أن تكون القيمة المدخلة بين 0 و 3 (شاملة 0 و 3). ضبط هذه القيمة إلى 0 يعني أن stdDev غير محدد. القيمة الافتراضية هي 0. |
| [SetStdDev](./setstddev/) | احصل أو عيّن عدد الانحرافات المعيارية لتضمينها فوق أو تحت المتوسط في قاعدة التنسيق الشرطي. يجب أن تكون القيمة المدخلة بين 0 و 3 (شاملة 0 و 3). ضبط هذه القيمة إلى 0 يعني أن stdDev غير محدد. القيمة الافتراضية هي 0. |
