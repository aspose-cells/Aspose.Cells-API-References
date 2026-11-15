---
title: "فئة WorkbookRender"
linktitle: "WorkbookRender"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "WorkbookRender فئة. يغلف الكائن الذي يمثل workbookrender في Go."
type: docs
weight: 200
url: /ar/go-cpp/workbookrender/
---

## WorkbookRender class

يمثل تصيير مصنف. يجب استخدام مُنشئ هذه الفئة بعد تعديل إعدادات الصفحة، نمط الخلية.

```go

type WorkbookRender struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewWorkbookRender](./newworkbookrender/) | بنية WorkbookRender |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetPageCount](./getpagecount/) | يحصل على إجمالي عدد الصفحات في workbook. |
| [GetPageSizeInch](./getpagesizeinch/) | احصل على حجم الصفحة بالبوصة للصورة الناتجة. |
| [ToImage](./toimage/) | قم بتصوير كامل workbook كـ Tiff Image إلى stream. |
| [ToImage_String](./toimage_string/) | قم بتصوير كامل workbook كـ Tiff Image إلى ملف. |
| [ToImage_Int_String](./toimage_int_string/) | قم بتصوير صفحة معينة إلى ملف. |
| [ToImage_Int](./toimage_int/) | قم بتصوير صفحة معينة إلى stream. |
| [Dispose](./dispose/) | يطلق الموارد التي تم إنشاؤها واستخدامها للتصوير. |
