---
title: "Enum PdfCustomPropertiesExport"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Rendering.PdfCustomPropertiesExport enum. Specifica il modo in cui CustomDocumentPropertyCollection vengono esportate in un file PDF"
type: docs
url: /it/net/aspose.cells.rendering/pdfcustompropertiesexport/
---
## PdfCustomPropertiesExport enumeration

Specifica il modo in cui [`CustomDocumentPropertyCollection`](../../aspose.cells.properties/customdocumentpropertycollection/) vengono esportate in un file PDF.

```csharp
public enum PdfCustomPropertiesExport
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Nessuna proprietà personalizzata viene esportata. |
| Standard | `1` | Le proprietà personalizzate vengono esportate come voci nel dizionario Info. |

### Esempi

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
            // Crea una cartella di lavoro e aggiungi alcuni dati
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello Aspose");
            worksheet.Cells["A2"].PutValue("This is a sample document");

            // Imposta alcune proprietà personalizzate
            workbook.Worksheets.CustomDocumentProperties.Add("Author", "John Doe");
            workbook.Worksheets.CustomDocumentProperties.Add("Subject", "Sample PDF Export");

            // Crea le opzioni di salvataggio PDF
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Imposta l'opzione di esportazione delle proprietà personalizzate
            saveOptions.CustomPropertiesExport = PdfCustomPropertiesExport.Standard;

            // Salva la cartella di lavoro in PDF
            workbook.Save("PdfCustomPropertiesExportExample.pdf", saveOptions);

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


