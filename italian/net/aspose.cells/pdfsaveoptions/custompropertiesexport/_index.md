---
title: "PdfSaveOptions.CustomPropertiesExport"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PdfSaveOptions proprietà. Ottiene o imposta un valore che determina il modo in cui CustomDocumentPropertyCollection vengono esportati nel file PDF. Il valore predefinito è None"
type: docs
url: /it/net/aspose.cells/pdfsaveoptions/custompropertiesexport/
---
## PdfSaveOptions.CustomPropertiesExport property

Ottiene o imposta un valore che determina il modo in cui [`CustomDocumentPropertyCollection`](../../../aspose.cells.properties/customdocumentpropertycollection/) vengono esportati nel file PDF. Il valore predefinito è None.

```csharp
public PdfCustomPropertiesExport CustomPropertiesExport { get; set; }
```

### Esempi

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

### Vedi anche

* enum [PdfCustomPropertiesExport](../../../aspose.cells.rendering/pdfcustompropertiesexport/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


