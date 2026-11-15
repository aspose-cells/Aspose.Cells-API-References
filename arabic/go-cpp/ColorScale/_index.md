---
title: "فئة ColorScale"
linktitle: "ColorScale"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة ColorScale. تغلف الكائن الذي يمثل colorscale في Go."
type: docs
weight: 200
url: /ar/go-cpp/colorscale/
---

## ColorScale class

وصف قاعدة تنسيق الشرطية ColorScale. تنشئ قاعدة التنسيق الشرطي هذه مقياس ألوان متدرج على الخلايا.

```go

type ColorScale struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetIs3ColorScale](./getis3colorscale/) | يشير إلى ما إذا كان التنسيق الشرطي هو مقياس ألوان ثلاثي. |
| [SetIs3ColorScale](./setis3colorscale/) | يشير إلى ما إذا كان التنسيق الشرطي هو مقياس ألوان ثلاثي. |
| [GetMinCfvo](./getmincfvo/) | احصل على أو عيّن كائن القيمة الدنيا لهذا ColorScale. لا يمكن تعيين null أو CFValueObject من النوع FormatConditionValueType.Max إليه. |
| [GetMidCfvo](./getmidcfvo/) | احصل على أو عيّن كائن القيمة المتوسطة لهذا ColorScale. لا يمكن تعيين CFValueObject من النوع FormatConditionValueType.Max أو FormatConditionValueType.Min إليه. |
| [GetMaxCfvo](./getmaxcfvo/) | احصل على أو عيّن كائن القيمة القصوى لهذا ColorScale. لا يمكن تعيين null أو CFValueObject من النوع FormatConditionValueType.Min إليه. |
| [GetMinColor](./getmincolor/) | احصل على أو عيّن لون التدرج للقيمة الدنيا في النطاق. |
| [SetMinColor](./setmincolor/) | احصل على أو عيّن لون التدرج للقيمة الدنيا في النطاق. |
| [GetMidColor](./getmidcolor/) | احصل على أو عيّن لون التدرج للقيمة المتوسطة في النطاق. |
| [SetMidColor](./setmidcolor/) | احصل على أو عيّن لون التدرج للقيمة المتوسطة في النطاق. |
| [GetMaxColor](./getmaxcolor/) | احصل على أو عيّن لون التدرج للقيمة القصوى في النطاق. |
| [SetMaxColor](./setmaxcolor/) | احصل على أو عيّن لون التدرج للقيمة القصوى في النطاق. |
