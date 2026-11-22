---
title: "WorkbookSettings.ResourceProvider"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. تحصل وتضبط موفر التدفق للموارد الخارجية مثل تحميل بيانات الصورة للرسمة من النوع LinkToFile"
type: docs
url: /ar/net/aspose.cells/workbooksettings/resourceprovider/
---
## WorkbookSettings.ResourceProvider property

يحصل أو يضبط موفر الدفق للموارد الخارجية، مثل تحميل بيانات الصورة للصور من النوع "LinkToFile".

```csharp
public IStreamProvider ResourceProvider { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyResourceProviderDemo
    {
        public static void Run()
        {
            // إنشاء مصنف تجريبي
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف شكلاً نموذجياً لتوضيح موفر الموارد
            worksheet.Shapes.AddRectangle(1, 1, 100, 100, 200, 200);
            
            // ضبط موفر الموارد
            workbook.Settings.ResourceProvider = new MemoryStreamProvider();
            
            // احفظ الشكل كصورة باستخدام موفر الموارد
            string outputPath = "output_shape.png";
            worksheet.Shapes[0].ToImage(outputPath, new ImageOrPrintOptions());
            
            Console.WriteLine("Shape saved as image using ResourceProvider.");
        }
    }

    public class MemoryStreamProvider : IStreamProvider
    {
        public void CloseStream(StreamProviderOptions options)
        {
            options.Stream.Close();
        }

        public void InitStream(StreamProviderOptions options)
        {
            options.Stream = new FileStream(options.DefaultPath, FileMode.Create);
        }
    }
}
```

### انظر أيضًا

* interface [IStreamProvider](../../istreamprovider/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


