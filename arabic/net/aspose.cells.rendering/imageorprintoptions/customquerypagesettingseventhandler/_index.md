---
title: "ImageOrPrintOptions.CustomQueryPageSettingsEventHandler"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageOrPrintOptions. يمكن للعميل التحكم في إعدادات صفحة الطابعة عند طباعة كل صفحة باستخدام هذا EventHandler"
type: docs
url: /ar/net/aspose.cells.rendering/imageorprintoptions/customquerypagesettingseventhandler/
---
## ImageOrPrintOptions.CustomQueryPageSettingsEventHandler property

يمكن للعميل التحكم في إعدادات صفحة الطابعة عند طباعة كل صفحة باستخدام هذا EventHandler

```csharp
public QueryPageSettingsEventHandler CustomQueryPageSettingsEventHandler { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyCustomQueryPageSettingsEventHandlerDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "More Data";

            try
            {
                // أنشئ مثيلًا لـ ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // عرض بعض الخصائص المتاحة
                Console.WriteLine("Current HorizontalResolution: " + options.HorizontalResolution);
                Console.WriteLine("Current VerticalResolution: " + options.VerticalResolution);
                Console.WriteLine("Current ImageType: " + options.ImageType);

                // إظهار ضبط بعض الخصائص
                options.HorizontalResolution = 300;
                options.VerticalResolution = 300;
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

                // تحقق من تعيين الخصائص
                Console.WriteLine("Updated HorizontalResolution: " + options.HorizontalResolution);
                Console.WriteLine("Updated VerticalResolution: " + options.VerticalResolution);
                Console.WriteLine("Updated ImageType: " + options.ImageType);

                // إنشاء SheetRender لإظهار عملية التصيير
                SheetRender renderer = new SheetRender(worksheet, options);

                // احفظ المصنف
                workbook.Save("CustomQueryPageSettingsEventHandlerDemo.xlsx");

                Console.WriteLine("ImageOrPrintOptions demonstration completed");
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


