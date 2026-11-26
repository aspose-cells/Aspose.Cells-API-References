---
title: "LowCodePdfSaveOptions.PdfOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LowCodePdfSaveOptions. Las opciones para guardar el archivo PDF"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodepdfsaveoptions/pdfoptions/
---
## LowCodePdfSaveOptions.PdfOptions property

Las opciones para guardar el archivo PDF.

```csharp
public PdfSaveOptions PdfOptions { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodePdfSaveOptionsPropertyPdfOptionsDemo
    {
        public static void Run()
        {
            // Crear libro de trabajo de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("PDF Options Demo");

            // Crear opciones de guardado PDF con configuraciones personalizadas
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions
            {
                Compliance = PdfCompliance.PdfA1b,
                OnePagePerSheet = true
            };

            // Crear opciones de guardado PDF de bajo código y asignar las opciones PDF
            LowCodePdfSaveOptions lowCodePdfSaveOptions = new LowCodePdfSaveOptions
            {
                OutputFile = "output.pdf",
                PdfOptions = pdfSaveOptions
            };

            // Guardar usando opciones de bajo código
            workbook.Save(lowCodePdfSaveOptions.OutputFile, lowCodePdfSaveOptions.PdfOptions);

            Console.WriteLine("PDF saved with custom options.");
        }
    }
}
```

### Ver también

* class [PdfSaveOptions](../../../aspose.cells/pdfsaveoptions/)
* class [LowCodePdfSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


