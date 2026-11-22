---
title: "HtmlSaveOptions.AddTooltipText"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "HtmlSaveOptions property. يشير إلى ما إذا كان يتم إضافة نص تلميح عندما لا يمكن عرض البيانات بالكامل. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/addtooltiptext/
---
## HtmlSaveOptions.AddTooltipText property

يشير إلى ما إذا كان يتم إضافة نص تلميح عندما لا يمكن عرض البيانات بالكامل. القيمة الافتراضية هي false.

```csharp
public bool AddTooltipText { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyAddTooltipTextDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // حدد نصًا طويلًا سيتجاوز عرض الخلية
            worksheet.Cells["A1"].PutValue("This is a long text that will exceed cell width and need tooltip");
            worksheet.Cells.SetColumnWidth(0, 10); // Set narrow column width
            
            // تكوين خيارات حفظ HTML مع تلميح
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.AddTooltipText = true;
            
            // احفظ المصنف
            string outputPath = "output_with_tooltip.html";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("File saved with tooltips: " + outputPath);
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


