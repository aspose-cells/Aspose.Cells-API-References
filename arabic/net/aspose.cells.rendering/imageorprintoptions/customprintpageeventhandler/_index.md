---
title: "ImageOrPrintOptions.CustomPrintPageEventHandler"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageOrPrintOptions. يمكن للعميل إخراج خاص إلى الطابعة عند طباعة كل صفحة باستخدام هذا EventHandler"
type: docs
url: /ar/net/aspose.cells.rendering/imageorprintoptions/customprintpageeventhandler/
---
## ImageOrPrintOptions.CustomPrintPageEventHandler property

يمكن للعميل إخراج خاص إلى الطابعة عند طباعة كل صفحة باستخدام هذا EventHandler

```csharp
public PrintPageEventHandler CustomPrintPageEventHandler { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyCustomPrintPageEventHandlerDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].Value = "Sample Data for Printing";
            worksheet.Cells["A2"].Value = "This demonstrates printing options";

            try
            {
                // أنشئ مثيلًا لـ ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // تكوين خيارات الطباعة
                options.PrintWithStatusDialog = true;
                options.HorizontalResolution = 300;
                options.VerticalResolution = 300;

                // عرض خيارات الطباعة الحالية
                Console.WriteLine($"PrintWithStatusDialog: {options.PrintWithStatusDialog}");
                Console.WriteLine($"HorizontalResolution: {options.HorizontalResolution}");
                Console.WriteLine($"VerticalResolution: {options.VerticalResolution}");

                // إنشاء SheetRender لتوضيح الطباعة
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // تحويل إلى صورة لعرض الطباعة
                sheetRender.ToImage(0, "output.png");
                Console.WriteLine("Rendering completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


