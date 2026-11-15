---
title: "فئة PivotItem"
linktitle: "PivotItem"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة PivotItem. تغلف الكائن الذي يمثل pivotitem في Go."
type: docs
weight: 200
url: /ar/go-cpp/pivotitem/
---

## PivotItem class

يمثل عنصرًا في تقرير PivotField.

```go

type PivotItem struct  {
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
| [IsHidden](./ishidden/) | يحصل ويضبط ما إذا كان عنصر المحور مخفيًا. |
| [SetIsHidden](./setishidden/) | يحصل ويضبط ما إذا كان عنصر المحور مخفيًا. |
| [GetPosition](./getposition/) | تحديد فهرس هذا العنصر في جميع PivotItems الخاصة بالحقل. |
| [SetPosition](./setposition/) | تحديد فهرس هذا العنصر في جميع PivotItems الخاصة بالحقل. |
| [GetPositionInSameParentNode](./getpositioninsameparentnode/) | تحديد فهرس الموقع في PivotItems تحت نفس العقدة الأصلية. |
| [SetPositionInSameParentNode](./setpositioninsameparentnode/) | تحديد فهرس الموقع في PivotItems تحت نفس العقدة الأصلية. |
| [Move](./move/) | ينقل العنصر للأعلى أو للأسفل |
| [IsDetailHidden](./isdetailhidden/) | يحصل ويضبط ما إذا كان تفصيل هذا العنصر المحوري مخفيًا. |
| [SetIsDetailHidden](./setisdetailhidden/) | يحصل ويضبط ما إذا كان تفصيل هذا العنصر المحوري مخفيًا. |
| [IsCalculatedItem](./iscalculateditem/) | يشير إلى ما إذا كان هذا العنصر المحوري عنصر صيغة محسوبة. |
| [GetFormula](./getformula/) | يحصل على صيغة هذا العنصر المحسوب. يعمل فقط عندما يكون هذا العنصر عنصرًا محسوبًا. |
| [IsMissing](./ismissing/) | يشير إلى ما إذا كان العنصر قد أُزيل من مصدر البيانات. |
| [GetStringValue](./getstringvalue/) | يحصل على القيمة النصية للعنصر المحوري إذا كانت القيمة فارغة، سيعيد \"\" |
| [GetDoubleValue](./getdoublevalue/) | يحصل على القيمة العشرية للعنصر المحوري. إذا كانت القيمة فارغة أو ليست رقمًا، سيعيد 0. |
| [GetDateTimeValue](./getdatetimevalue/) | يحصل على قيمة التاريخ والوقت للعنصر المحوري. إذا كانت القيمة فارغة، سيعيد DateTime.MinValue. |
| [GetValue](./getvalue/) | يحصل على قيمة العنصر المحوري |
| [GetName](./getname/) | يحصل على اسم العنصر المحوري. |
| [SetName](./setname/) | يحصل على اسم العنصر المحوري. |
