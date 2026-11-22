---
title: "الفئة WorkbookRender"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Rendering.WorkbookRender. تمثّل عملية عرض المصنف. يجب استخدام منشئ هذه الفئة بعد تعديل نمط خلية إعداد الصفحة"
type: docs
url: /ar/net/aspose.cells.rendering/workbookrender/
---
## WorkbookRender class

يمثل عرضًا للمصنف. يجب استخدام منشئ هذه الفئة بعد تعديل إعدادات الصفحة (pagesetup) ونمط الخلية.

```csharp
public class WorkbookRender
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [WorkbookRender](workbookrender/)(Workbook, ImageOrPrintOptions) | بناء WorkbookRender |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [PageCount](../../aspose.cells.rendering/workbookrender/pagecount/) { get; } | يحصل على إجمالي عدد الصفحات في المصنف. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [CustomPrint](../../aspose.cells.rendering/workbookrender/customprint/)(bool, PrintPageEventArgs) | يمكن للعميل التحكم في إعدادات صفحة الطابعة عند طباعة كل صفحة باستخدام هذه الدالة. |
| [Dispose](../../aspose.cells.rendering/workbookrender/dispose/)() | يطلق الموارد التي تم إنشاؤها واستخدامها في عملية العرض. |
| [GetPageSizeInch](../../aspose.cells.rendering/workbookrender/getpagesizeinch/)(int) | احصل على حجم الصفحة بالبوصة للصورة الناتجة. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage)(int) | اعرض صفحة معينة إلى كائن Bitmap. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_3)(Stream) | اعرض المصنف بالكامل كصورة Tiff إلى تدفق. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_4)(string) | اعرض المصنف بالكامل كصورة Tiff إلى ملف. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_1)(int, Stream) | اعرض صفحة معينة إلى تدفق. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_2)(int, string) | اعرض صفحة معينة إلى ملف. |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter)(PrinterSettings) | اعرض المصنف إلى الطابعة |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_2)(string) | اعرض المصنف إلى الطابعة |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_1)(PrinterSettings, string) | اعرض المصنف إلى الطابعة |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_4)(string, string) | اعرض المصنف إلى الطابعة |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_3)(string, int, int) | (**Obsolete.**) اعرض المصنف إلى الطابعة |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassWorkbookRenderDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات عينة واضبط حجم الصفحة
            worksheet.Cells["A1"].PutValue("Workbook Render Demo");
            worksheet.PageSetup.PaperSize = PaperSizeType.PaperLetter;

            // إنشاء خيارات الصورة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // إنشاء عرض دفتر العمل والحصول على حجم الصفحة
            WorkbookRender render = new WorkbookRender(workbook, options);
            float[] pageSize = render.GetPageSizeInch(0);
            
            // أخرج النتائج
            Console.WriteLine($"Page Width: {pageSize[0]} inches");
            Console.WriteLine($"Page Height: {pageSize[1]} inches");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


