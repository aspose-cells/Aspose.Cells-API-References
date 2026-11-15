---
title: "فئة SheetRender"
linktitle: "SheetRender"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة SheetRender. تغلف الكائن الذي يمثل sheetrender في Go."
type: docs
weight: 200
url: /ar/go-cpp/sheetrender/
---

## SheetRender class

يمثل تصيير ورقة عمل يمكنه تصيير ورقة العمل إلى صور مختلفة مثل (BMP, PNG, JPEG, TIFF..). يجب استخدام مُنشئ هذه الفئة بعد تعديل إعدادات الصفحة، نمط الخلية.

```go

type SheetRender struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewSheetRender](./newsheetrender/) | إنشاء SheetRender، يحتاج إلى ورقة عمل و ImageOrPrintOptions كمعاملات |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetPageCount](./getpagecount/) | يحصل على إجمالي عدد الصفحات لورقة العمل الحالية. |
| [GetPageScale](./getpagescale/) | يحصل على مقياس الصفحة المحسوب للورقة. يعيد المقياس المحدد إذا تم تعيين PageSetup.Zoom. وإلا، يعيد المقياس المحسوب وفقًا لـ PageSetup.FitToPagesWide و PageSetup.FitToPagesTall. |
| [GetPageSizeInch](./getpagesizeinch/) | احصل على حجم الصفحة بالبوصة للصورة الناتجة. |
| [ToImage_Int_String](./toimage_int_string/) | قم بتصوير صفحة معينة إلى ملف. |
| [ToImage_Int](./toimage_int/) | قم بتصوير صفحة معينة إلى stream. |
| [ToTiff](./totiff/) | تصدير كامل ورقة العمل كصورة Tiff إلى تدفق. |
| [ToTiff_String](./totiff_string/) | تصدير كامل ورقة العمل كصورة Tiff إلى ملف. |
| [Dispose](./dispose/) | يطلق الموارد التي تم إنشاؤها واستخدامها للتصوير. |
