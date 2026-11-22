---
title: "Class GridSheetRender"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.GridDesktop.Data.GridSheetRender class. تمثل عرض ورقة عمل يمكنه تصيير الورقة إلى صور مختلفة مثل BMP PNG JPEG TIFF.. يجب استخدام منشئ هذه الفئة بعد تعديل نمط خلية إعداد الصفحة"
type: docs
url: /ar/net/aspose.cells.griddesktop.data/gridsheetrender/
---
## GridSheetRender class

يمثل عرض ورقة عمل يمكنه تحويل ورقة العمل إلى صور مختلفة مثل (BMP, PNG, JPEG, TIFF..). يجب استخدام منشئ هذه الفئة بعد تعديل إعدادات الصفحة (pagesetup) ونمط الخلية.

```csharp
public class GridSheetRender
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [GridSheetRender](gridsheetrender/)(Worksheet, GridImageOrPrintOptions) | إنشاء SheetRender، يحتاج إلى ورقة عمل و ImageOrPrintOptions كمعلمات |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [PageCount](../../aspose.cells.griddesktop.data/gridsheetrender/pagecount/) { get; } | يحصل على إجمالي عدد الصفحات في ورقة العمل الحالية. |
| [PageScale](../../aspose.cells.griddesktop.data/gridsheetrender/pagescale/) { get; } | يحصل على مقياس الصفحة المحسوب للورقة. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetPageSizeInch](../../aspose.cells.griddesktop.data/gridsheetrender/getpagesizeinch/)(int) | احصل على حجم الصفحة بالبوصة للصورة الناتجة. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage)(int) | اعرض صفحة معينة إلى كائن Bitmap. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_3)(int, Stream) | اعرض صفحة معينة إلى تدفق. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_4)(int, string) | اعرض صفحة معينة إلى ملف. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_1)(int, Graphics, float, float) | عرض صفحة معينة إلى Graphics |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_2)(int, Graphics, float, float, float, float) | عرض صفحة معينة إلى Graphics |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter)(PrinterSettings) | عرض ورقة العمل إلى Printer |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter_2)(string) | عرض ورقة العمل إلى Printer |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter_1)(PrinterSettings, string) | عرض ورقة العمل إلى Printer |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter_3)(string, string) | عرض ورقة العمل إلى Printer |
| [ToTiff](../../aspose.cells.griddesktop.data/gridsheetrender/totiff/#totiff)(Stream) | عرض كامل ورقة العمل كصورة Tiff إلى تدفق. |
| [ToTiff](../../aspose.cells.griddesktop.data/gridsheetrender/totiff/#totiff_1)(string) | عرض كامل ورقة العمل كصورة Tiff إلى ملف. |

### انظر أيضًا

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


