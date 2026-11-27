---
title: "PdfSaveOptions.CustomPropertiesExport"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfSaveOptions-egenskap. Hämtar eller anger ett värde som bestämmer hur CustomDocumentPropertyCollection exporteras till PDF‑fil. Standardvärdet är None"
type: docs
url: /sv/net/aspose.cells/pdfsaveoptions/custompropertiesexport/
---
## PdfSaveOptions.CustomPropertiesExport property

Hämtar eller anger ett värde som bestämmer hur [`CustomDocumentPropertyCollection`](../../../aspose.cells.properties/customdocumentpropertycollection/) exporteras till PDF‑fil. Standardvärdet är None.

```csharp
public PdfCustomPropertiesExport CustomPropertiesExport { get; set; }
```

### Exempel

```csharp
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyCustomPropertiesExportDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello Aspose");
            worksheet.Cells["A2"].PutValue("Sample PDF Export");

            workbook.CustomDocumentProperties.Add("Author", "John Doe");
            workbook.CustomDocumentProperties.Add("Subject", "Aspose.Cells Example");

            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.CustomPropertiesExport = PdfCustomPropertiesExport.Standard;

            workbook.Save("PdfCustomPropertiesExportDemo.pdf", saveOptions);
        }
    }
}
```

### Se även

* enum [PdfCustomPropertiesExport](../../../aspose.cells.rendering/pdfcustompropertiesexport/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


