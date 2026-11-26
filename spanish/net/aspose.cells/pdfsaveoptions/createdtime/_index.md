---
title: "PdfSaveOptions.CreatedTime"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PdfSaveOptions. Obtiene y establece la hora de generación del documento pdf"
type: docs
url: /es/net/aspose.cells/pdfsaveoptions/createdtime/
---
## PdfSaveOptions.CreatedTime property

Obtiene o establece la hora de generación del documento pdf.

```csharp
public DateTime CreatedTime { get; set; }
```

### Observaciones

si no se establece, será la hora de generación del pdf.

### Ejemplos

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

### Ver también

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


