---
title: "PdfSaveOptions.CreatedTime"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PdfSaveOptions. تحصل وتعيّن وقت إنشاء مستند PDF"
type: docs
url: /ar/net/aspose.cells/pdfsaveoptions/createdtime/
---
## PdfSaveOptions.CreatedTime property

يحصل على ويضبط وقت إنشاء مستند PDF.

```csharp
public DateTime CreatedTime { get; set; }
```

### ملاحظات

إذا لم يتم تعيينه، فسيكون وقت إنشاء ملف PDF.

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyCreatedTimeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("PDF with CreatedTime demonstration");

            PdfSaveOptions saveOptions = new PdfSaveOptions
            {
                CreatedTime = DateTime.Now,
                Compliance = PdfCompliance.PdfA1b
            };

            string outputPath = "OutputWithCreatedTime.pdf";
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine($"PDF saved with CreatedTime: {saveOptions.CreatedTime}");
        }
    }
}
```

### انظر أيضًا

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


