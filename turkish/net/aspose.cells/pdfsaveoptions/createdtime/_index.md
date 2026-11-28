---
title: "PdfSaveOptions.CreatedTime"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PdfSaveOptions özelliği. PDF belgesinin oluşturulma zamanını alır ve ayarlar."
type: docs
url: /tr/net/aspose.cells/pdfsaveoptions/createdtime/
---
## PdfSaveOptions.CreatedTime property

PDF belgesinin oluşturulma zamanını alır ve ayarlar.

```csharp
public DateTime CreatedTime { get; set; }
```

### Açıklamalar

Eğer ayarlanmamışsa, pdf'nin oluşturulma zamanı olacaktır.

### Örnekler

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

### Ayrıca Bakınız

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


