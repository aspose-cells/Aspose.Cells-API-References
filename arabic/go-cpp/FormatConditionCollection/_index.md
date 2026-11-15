---
title: "فئة FormatConditionCollection"
linktitle: "FormatConditionCollection"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة FormatConditionCollection. تغلف الكائن الذي يمثل formatconditioncollection في Go."
type: docs
weight: 200
url: /ar/go-cpp/formatconditioncollection/
---

## FormatConditionCollection class

يمثل تنسيقًا شرطيًا. يمكن أن يحتوي FormatConditions على ما يصل إلى ثلاثة تنسيقات شرطية.

```go

type FormatConditionCollection struct  {
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
| [Add](./add/) | يضيف شرط تنسيق ونطاق الخلايا المتأثر إلى FormatConditions. يمكن أن يحتوي FormatConditions على ما يصل إلى ثلاثة تنسيقات شرطية. لا يُسمح بالإشارات إلى الأوراق الأخرى في صيغ التنسيق الشرطي. |
| [AddArea](./addarea/) | يضيف نطاق خلايا مُنسق شرطياً. |
| [AddCondition_FormatConditionType_OperatorType_String_String](./addcondition_formatconditiontype_operatortype_string_string/) | يضيف شرط تنسيق. |
| [AddCondition_FormatConditionType](./addcondition_formatconditiontype/) | أضف شرط تنسيق. |
| [GetCount](./getcount/) | يحصل على عدد الشروط. |
| [GetRangeCount](./getrangecount/) | يحصل على عدد النطاقات المُنسقة شرطياً. |
| [Get](./get/) | يحصل على شرط التنسيق حسب الفهرس. |
| [GetCellArea](./getcellarea/) | يحصل على نطاق الخلايا المُنسقة شرطياً حسب الفهرس. |
| [RemoveArea_Int](./removearea_int/) | يزيل نطاق الخلايا المُنسقة شرطياً حسب الفهرس. |
| [RemoveArea_Int_Int_Int_Int](./removearea_int_int_int_int/) | إزالة التنسيق الشرطي في النطاق. |
| [RemoveCondition](./removecondition/) | يزيل شرط التنسيق حسب الفهرس. |
