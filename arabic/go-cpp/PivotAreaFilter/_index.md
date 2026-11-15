---
title: "فئة PivotAreaFilter"
linktitle: "PivotAreaFilter"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة PivotAreaFilter. تغلف الكائن الذي يمثل pivotareafilter في Go."
type: docs
weight: 200
url: /ar/go-cpp/pivotareafilter/
---

## PivotAreaFilter class

يمثل مرشح <see cref=\"PivotArea\"/> لـ <see cref=\"PivotTable\"/>.

```go

type PivotAreaFilter struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewPivotAreaFilter](./newpivotareafilter/) | البناء الافتراضي. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [IsSubtotalSet](./issubtotalset/) | يحصل على أي مجموع فرعي تم تعيينه لهذا الفلتر. |
| [SetSubtotals](./setsubtotals/) | المجموع الفرعي للفلتر. |
| [GetFieldIndex](./getfieldindex/) | يحصل على فهرس الحقل في الحقول المصدر التي يشير إليها هذا الفلتر. قيمة -2 تشير إلى حقل القيم. |
| [GetSelected](./getselected/) | يشير إلى ما إذا كان لهذا الحقل تحديد. يعمل فقط عندما تكون PivotTable في وضع المخطط التفصيلي. |
| [SetSelected](./setselected/) | يشير إلى ما إذا كان لهذا الحقل تحديد. يعمل فقط عندما تكون PivotTable في وضع المخطط التفصيلي. |
