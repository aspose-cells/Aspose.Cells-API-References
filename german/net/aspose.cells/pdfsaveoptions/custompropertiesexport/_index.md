---
title: "PdfSaveOptions.CustomPropertiesExport"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PdfSaveOptions-Eigenschaft. Liest oder setzt einen Wert, der bestimmt, wie CustomDocumentPropertyCollection in eine PDF-Datei exportiert werden. Standardwert ist None."
type: docs
url: /de/net/aspose.cells/pdfsaveoptions/custompropertiesexport/
---
## PdfSaveOptions.CustomPropertiesExport property

Liest oder setzt einen Wert, der bestimmt, wie [`CustomDocumentPropertyCollection`](../../../aspose.cells.properties/customdocumentpropertycollection/) in eine PDF-Datei exportiert werden. Standardwert ist None.

```csharp
public PdfCustomPropertiesExport CustomPropertiesExport { get; set; }
```

### Beispiele

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

### Siehe auch

* enum [PdfCustomPropertiesExport](../../../aspose.cells.rendering/pdfcustompropertiesexport/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


