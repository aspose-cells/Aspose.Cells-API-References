---
title: "Enum PdfCustomPropertiesExport"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Rendering.PdfCustomPropertiesExport enum. Anger hur CustomDocumentPropertyCollection exporteras till PDF-fil"
type: docs
url: /sv/net/aspose.cells.rendering/pdfcustompropertiesexport/
---
## PdfCustomPropertiesExport enumeration

Anger hur [`CustomDocumentPropertyCollection`](../../aspose.cells.properties/customdocumentpropertycollection/) exporteras till PDF-fil.

```csharp
public enum PdfCustomPropertiesExport
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Inga anpassade egenskaper exporteras. |
| Standard | `1` | Anpassade egenskaper exporteras som poster i Info-ordboken. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PdfCustomPropertiesExportDemo
    {
        public static void PdfCustomPropertiesExportExample()
        {
            // Skapa en arbetsbok och lägg till lite data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello Aspose");
            worksheet.Cells["A2"].PutValue("This is a sample document");

            // Ange några anpassade egenskaper
            workbook.Worksheets.CustomDocumentProperties.Add("Author", "John Doe");
            workbook.Worksheets.CustomDocumentProperties.Add("Subject", "Sample PDF Export");

            // Skapa PDF-sparalternativ
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Ställ in exportalternativet för anpassade egenskaper
            saveOptions.CustomPropertiesExport = PdfCustomPropertiesExport.Standard;

            // Spara arbetsboken som PDF
            workbook.Save("PdfCustomPropertiesExportExample.pdf", saveOptions);

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


