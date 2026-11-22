---
title: "HtmlSaveOptions.WorksheetScalable"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. تشير إلى ما إذا كان سيتم تكبير أو تصغير html عبر مستوى تكبير ورقة العمل عند حفظ الملف إلى html. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/worksheetscalable/
---
## HtmlSaveOptions.WorksheetScalable property

يشير إلى ما إذا كان يتم تكبير أو تصغير HTML عبر مستوى تكبير ورقة العمل عند حفظ الملف إلى HTML، القيمة الافتراضية هي false.

```csharp
public bool WorksheetScalable { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyWorksheetScalableDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // تعيين خيارات حفظ HTML باستخدام خاصية WorksheetScalable
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.WorksheetScalable = true;
            
            // حفظ دفتر العمل مع خيارات HTML
            string outputPath = "output.html";
            workbook.Save(outputPath, options);
            
            // تحقق من أن الناتج يحتوي على نمط التحجيم
            string htmlContent = File.ReadAllText(outputPath);
            Console.WriteLine("HTML contains scaling: " + htmlContent.Contains("transform: scale"));
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


