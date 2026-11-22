---
title: "الفئة SheetRender"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Rendering.SheetRender. تمثل عملية عرض ورقة العمل التي يمكنها تحويل ورقة العمل إلى صور مختلفة مثل BMP و PNG و JPEG و TIFF.. يجب استخدام مُنشئ هذه الفئة بعد تعديل نمط الخلية في إعدادات الصفحة"
type: docs
url: /ar/net/aspose.cells.rendering/sheetrender/
---
## SheetRender class

يمثل عرض ورقة عمل يمكنه تحويل ورقة العمل إلى صور مختلفة مثل (BMP, PNG, JPEG, TIFF..). يجب استخدام منشئ هذه الفئة بعد تعديل إعدادات الصفحة (pagesetup) ونمط الخلية.

```csharp
public class SheetRender
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [SheetRender](sheetrender/)(Worksheet, ImageOrPrintOptions) | إنشاء SheetRender، يحتاج إلى ورقة عمل و ImageOrPrintOptions كمعلمات |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [PageCount](../../aspose.cells.rendering/sheetrender/pagecount/) { get; } | يحصل على إجمالي عدد الصفحات في ورقة العمل الحالية. |
| [PageScale](../../aspose.cells.rendering/sheetrender/pagescale/) { get; } | يحصل على مقياس الصفحة المحسوب للورقة. يُعيد المقياس المحدد إذا كان [`Zoom`](../../aspose.cells/pagesetup/zoom/) مُعيّنًا. وإلا، يُعيد المقياس المحسوب وفقًا لـ [`FitToPagesWide`](../../aspose.cells/pagesetup/fittopageswide/) و [`FitToPagesTall`](../../aspose.cells/pagesetup/fittopagestall/). |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [CustomPrint](../../aspose.cells.rendering/sheetrender/customprint/)(bool, PrintPageEventArgs) | يمكن للعميل التحكم في إعدادات صفحة الطابعة عند طباعة كل صفحة باستخدام هذه الدالة. |
| [Dispose](../../aspose.cells.rendering/sheetrender/dispose/)() | يطلق الموارد التي تم إنشاؤها واستخدامها في عملية العرض. |
| [GetPageSizeInch](../../aspose.cells.rendering/sheetrender/getpagesizeinch/)(int) | احصل على حجم الصفحة بالبوصة للصورة الناتجة. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage)(int) | اعرض صفحة معينة إلى كائن Bitmap. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_3)(int, Stream) | اعرض صفحة معينة إلى تدفق. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_4)(int, string) | اعرض صفحة معينة إلى ملف. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_1)(int, Graphics, float, float) | عرض صفحة معينة إلى Graphics |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_2)(int, Graphics, float, float, float, float) | عرض صفحة معينة إلى Graphics |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter)(PrinterSettings) | عرض ورقة العمل إلى Printer |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_2)(string) | عرض ورقة العمل إلى Printer |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_1)(PrinterSettings, string) | عرض ورقة العمل إلى Printer |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_4)(string, string) | عرض ورقة العمل إلى Printer |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_3)(string, int, int) | (**Obsolete.**) عرض ورقة العمل إلى Printer |
| [ToTiff](../../aspose.cells.rendering/sheetrender/totiff/#totiff)(Stream) | عرض كامل ورقة العمل كصورة Tiff إلى تدفق. |
| [ToTiff](../../aspose.cells.rendering/sheetrender/totiff/#totiff_1)(string) | عرض كامل ورقة العمل كصورة Tiff إلى ملف. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassSheetRenderDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // أضف بيانات تجريبية
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // تكوين إعداد الصفحة
            PageSetup pageSetup = sheet.PageSetup;
            pageSetup.PrintArea = "1:10";
            pageSetup.SetFitToPages(1, 1);

            // إنشاء SheetRender وعرض الوظيفة الأساسية
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            SheetRender sr = new SheetRender(sheet, options);
            
            Console.WriteLine($"Number of pages: {sr.PageCount}");
            Console.WriteLine($"Page scale: {sr.PageScale * 100}%");
            
            // عرض الصفحة الأولى إلى صورة (توضيح)
            sr.ToImage(0, "output_page1.png");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


