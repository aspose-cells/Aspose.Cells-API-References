---
title: "RowCollection فئة"
linktitle: "RowCollection"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "RowCollection فئة. تغلف الكائن الذي يمثل rowcollection في Go."
type: docs
weight: 200
url: /ar/go-cpp/rowcollection/
---

## RowCollection class

يجمع كائنات <see cref="Row"/> التي تمثل الصفوف الفردية في ورقة العمل.

```go

type RowCollection struct  {
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
| [GetCount](./getcount/) | يحصل على عدد الصفوف في هذه المجموعة. |
| [GetEnumerator](./getenumerator/) | يحصل على مُعدِّد يتنقل عبر الصفوف في هذه المجموعة. |
| [GetEnumerator_Bool_Bool](./getenumerator_bool_bool/) | يحصل على مُعدِّد يتنقل عبر الصفوف في هذه المجموعة. |
| [GetRowByIndex](./getrowbyindex/) | يحصل على كائن الصف بواسطة الموضع في القائمة. |
| [Get](./get/) | يحصل على كائن Row بواسطة فهرس الصف المعطى. سيتم إنشاء كائن Row للفهرس المعطى إذا لم يكن موجودًا مسبقًا. |
| [Clear](./clear/) | امسح جميع الصفوف والخلايا. |
| [RemoveAt](./removeat/) | أزل عنصر الصف عند الفهرس (الموضع) المحدد في هذه المجموعة. |
