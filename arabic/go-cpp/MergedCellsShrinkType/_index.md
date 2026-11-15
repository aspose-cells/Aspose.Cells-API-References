---
title: "MergedCellsShrinkType تعداد"
linktitle: "MergedCellsShrinkType"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "تعداد MergedCellsShrinkType. يغلف الكائن الذي يمثل mergedcellsshrinktype في Go."
type: docs
weight: 200
url: /ar/go-cpp/mergedcellsshrinktype/
---

## MergedCellsShrinkType Enum

يمثل الاستراتيجية لتقليص الخلايا المدمجة للعمليات مثل حذف الصفوف/الأعمدة الفارغة.

```go

type MergedCellsShrinkType int32


```

## الحقول

| حقل | الوصف |
| --- | --- |
| [None](./none/) | يترك الخلايا المدمجة كما هي دون أي تعديل. |
| [ShrinkToFit](./shrinktofit/) | يقوم بتقليص المنطقة المدمجة إذا لزم الأمر، عن طريق إزالة الصفوف من الأسفل أو الأعمدة من اليمين، مع ضمان بقاء جميع المحتويات مرئية. |
| [KeepHeaderOnly](./keepheaderonly/) | يحتفظ فقط بالصفوف/الأعمدة الرأسية للمنطقة المدمجة عندما لا تكون الخلية العليا اليسرى للمنطقة المدمجة فارغة. |
