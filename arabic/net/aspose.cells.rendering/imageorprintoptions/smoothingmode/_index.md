---
title: "ImageOrPrintOptions.SmoothingMode"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ImageOrPrintOptions. تحدد ما إذا كان يتم تطبيق تنعيم مضاد للتعرج على الخطوط والمنحنيات وحواف المناطق المملوءة. القيمة الافتراضية هي SmoothingMode.None"
type: docs
url: /ar/net/aspose.cells.rendering/imageorprintoptions/smoothingmode/
---
## ImageOrPrintOptions.SmoothingMode property

يحدد ما إذا كان يتم تطبيق التنعيم (إزالة التعرجات) على الخطوط والمنحنيات وحواف المناطق المملوءة. القيمة الافتراضية هي SmoothingMode.None

```csharp
public SmoothingMode SmoothingMode { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertySmoothingModeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].Value = "ImageOrPrintOptions Demo";
            worksheet.Cells["A2"].Value = "Sample Data";

            try
            {
                // أنشئ مثيلًا لـ ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // عرض بعض الخصائص المتاحة
                Console.WriteLine("HorizontalResolution: " + options.HorizontalResolution);
                Console.WriteLine("VerticalResolution: " + options.VerticalResolution);
                Console.WriteLine("ImageType: " + options.ImageType);

                // أنشئ SheetRender لتوضيح الخاصية
                SheetRender renderer = new SheetRender(worksheet, options);

                // قم بالتصيير إلى تدفق الذاكرة لتوضيح الوظيفة
                MemoryStream stream = new MemoryStream();
                renderer.ToImage(0, stream);

                Console.WriteLine("Sheet rendered successfully");
                Console.WriteLine("Image size: " + stream.Length + " bytes");

                // احفظ المصنف
                workbook.Save("ImageOrPrintOptionsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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


