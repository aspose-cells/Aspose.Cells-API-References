---
title: "PdfSaveOptions.CustomPropertiesExport"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PdfSaveOptions. Obtiene o establece un valor que determina la forma en que CustomDocumentPropertyCollection se exporta al archivo PDF. El valor predeterminado es None"
type: docs
url: /es/net/aspose.cells/pdfsaveoptions/custompropertiesexport/
---
## PdfSaveOptions.CustomPropertiesExport property

Obtiene o establece un valor que determina la forma en que [`CustomDocumentPropertyCollection`](../../../aspose.cells.properties/customdocumentpropertycollection/) se exporta al archivo PDF. El valor predeterminado es None.

```csharp
public PdfCustomPropertiesExport CustomPropertiesExport { get; set; }
```

### Ejemplos

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

### Ver también

* enum [PdfCustomPropertiesExport](../../../aspose.cells.rendering/pdfcustompropertiesexport/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


