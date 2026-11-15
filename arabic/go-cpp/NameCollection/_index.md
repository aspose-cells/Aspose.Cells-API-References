---
title: "فئة NameCollection"
linktitle: "NameCollection"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة NameCollection. تغلف الكائن الذي يمثل namecollection في Go."
type: docs
weight: 200
url: /ar/go-cpp/namecollection/
---

## NameCollection class

يمثل مجموعة من جميع كائنات <see cref=\"Name\"/> في جدول البيانات.

```go

type NameCollection struct  {
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
| [Add](./add/) | يعرف اسمًا جديدًا. |
| [Get_Int](./get_int/) | يحصل على عنصر Name في الفهرس المحدد. |
| [Filter](./filter/) | يحصل على جميع الأسماء المعرفة حسب النطاق. |
| [Get_String](./get_string/) | يحصل على عنصر Name بالاسم المحدد. |
| [Remove_stringArray](./remove_stringarray/) | إزالة مصفوفة من الأسماء |
| [Remove_String](./remove_string/) | إزالة الاسم. |
| [RemoveAt](./removeat/) | إزالة الاسم في الفهرس المحدد. |
| [Clear](./clear/) | إزالة جميع الأسماء المعرفة التي لا يتم الإشارة إليها من قبل الصيغ ومصدر البيانات. إذا تم الإشارة إلى الاسم المعرفة، نقوم فقط بتعيين Name.ReferTo إلى null وإخفائه. |
| [RemoveDuplicateNames](./removeduplicatenames/) | إزالة الأسماء المعرفة المكررة |
| [Sort](./sort/) | يقوم بترتيب الأسماء المعرفة. |
| [GetCount](./getcount/) | يحصل على عدد العناصر الموجودة في المثيل. |
