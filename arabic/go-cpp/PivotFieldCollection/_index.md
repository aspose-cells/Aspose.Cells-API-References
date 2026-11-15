---
title: "فئة PivotFieldCollection"
linktitle: "PivotFieldCollection"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة PivotFieldCollection. يحتوي على الكائن الذي يمثل pivotfieldcollection في Go."
type: docs
weight: 200
url: /ar/go-cpp/pivotfieldcollection/
---

## PivotFieldCollection class

يمثل مجموعة جميع كائنات PivotField في المناطق المختلفة لجدول محوري.

```go

type PivotFieldCollection struct  {
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
| [GetType](./gettype/) | يحصل على نوع PivotFields. |
| [Get_Int](./get_int/) | يحصل على كائن PivotField عند الفهرس المحدد. |
| [Get_String](./get_string/) | يحصل على كائن PivotField بالاسم المحدد. |
| [RemoveAt](./removeat/) | يزيل الحقل حسب الفهرس. فقط للمنطقة filter,row,column,data. |
| [AddByBaseIndex](./addbybaseindex/) | يضيف كائن PivotField إلى النوع المحدد PivotFields. |
| [Add](./add/) | يضيف كائن PivotField إلى النوع المحدد PivotFields. |
| [Insert](./insert/) | إدراج حقل pivot عند الفهرس المحدد. |
| [Clear](./clear/) | مسح جميع الحقول في PivotFieldCollection |
| [Remove](./remove/) | يزيل الحقل من المنطقة الحالية. |
| [Move](./move/) | ينقل PivotField من الموضع الحالي إلى الموضع الهدف |
| [GetCount](./getcount/) | يحصل على عدد العناصر الموجودة في المثيل. |
