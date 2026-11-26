---
title: "PdfSaveOptions.CreatedTime"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PdfSaveOptions. Получает и задает время создания pdf‑документа"
type: docs
url: /ru/net/aspose.cells/pdfsaveoptions/createdtime/
---
## PdfSaveOptions.CreatedTime property

Получает или задаёт время создания PDF‑документа.

```csharp
public DateTime CreatedTime { get; set; }
```

### Примечания

Если оно не будет установлено, будет использовано время создания pdf.

### Примеры

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

### См. также

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


