---
title: "DrawObject فئة"
linktitle: "DrawObject"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "DrawObject class. يغلف الكائن الذي يمثل drawobject في Go."
type: docs
weight: 200
url: /ar/go-cpp/drawobject/
---

## DrawObject class

سيتم تهيئة DrawObject وإرجاعه أثناء التصيير.

```go

type DrawObject struct  {
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
| [GetCell](./getcell/) | يشير إلى كائن Cell عند العرض. يمكن الوصول إلى جميع خصائص الخلية. |
| [GetShape](./getshape/) | يشير إلى كائن Shape عند العرض. يمكن الوصول إلى جميع خصائص الشكل. |
| [GetImageBytes](./getimagebytes/) | يشير إلى بايتات الصورة للـ Chart و Shape المرسومة عند العرض. |
| [GetType](./gettype/) | يشير إلى نوع DrawObject. |
| [GetCurrentPage](./getcurrentpage/) | يشير إلى فهرس الصفحة لـ DrawObject. فهرس الصفحة يبدأ من الصفر. يحتوي ورقة واحدة على عدة صفحات عند العرض. |
| [GetTotalPages](./gettotalpages/) | يشير إلى إجمالي الصفحات في العرض الحالي. |
| [GetSheetIndex](./getsheetindex/) | يشير إلى فهرس الورقة الحالية لـ DrawObject. |
