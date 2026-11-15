---
title: "فئة ColumnCollection"
linktitle: "ColumnCollection"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة ColumnCollection. تغلف الكائن الذي يمثل columncollection في Go."
type: docs
weight: 200
url: /ar/go-cpp/columncollection/
---

## ColumnCollection class

مجموعة من كائنات <see cref="Column"/> التي تمثل إعدادات الأعمدة الفردية في ورقة العمل. كائن Column يمثل فقط الإعدادات مثل عرض العمود، الأنماط، إلخ للعمود بأكمله، ولا علاقة له بوجود خلايا غير فارغة (بيانات) أو عدمها في العمود المقابل. و"Count" لهذه المجموعة يمثل فقط عدد كائنات Column التي تم إنشاءها في هذه المجموعة، ولا علاقة له بوجود خلايا غير فارغة (بيانات) أو عدمها في ورقة العمل.

```go

type ColumnCollection struct  {
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
| [GetColumnByIndex](./getcolumnbyindex/) | يحصل على كائن Column حسب الموقع في القائمة. |
| [Get](./get/) | يحصل على كائن Column حسب فهرس العمود. سيتم إنشاء كائن Column للفهرس المحدد إذا لم يكن موجودًا مسبقًا. |
| [GetCount](./getcount/) | يحصل على عدد العناصر الموجودة في المثيل. |
