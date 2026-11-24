---
title: "Enum PdfCustomPropertiesExport"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Rendering.PdfCustomPropertiesExport enum. Gibt an, wie CustomDocumentPropertyCollection in eine PDF-Datei exportiert werden"
type: docs
url: /de/net/aspose.cells.rendering/pdfcustompropertiesexport/
---
## PdfCustomPropertiesExport enumeration

Gibt an, wie [`CustomDocumentPropertyCollection`](../../aspose.cells.properties/customdocumentpropertycollection/) in eine PDF-Datei exportiert werden.

```csharp
public enum PdfCustomPropertiesExport
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Keine benutzerdefinierten Eigenschaften werden exportiert. |
| Standard | `1` | Benutzerdefinierte Eigenschaften werden als Einträge im Info-Wörterbuch exportiert. |

### Beispiele

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
            // Erstellen Sie eine Arbeitsmappe und fügen Sie einige Daten hinzu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello Aspose");
            worksheet.Cells["A2"].PutValue("This is a sample document");

            // Legen Sie einige benutzerdefinierte Eigenschaften fest
            workbook.Worksheets.CustomDocumentProperties.Add("Author", "John Doe");
            workbook.Worksheets.CustomDocumentProperties.Add("Subject", "Sample PDF Export");

            // PDF-Speicheroptionen erstellen
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Die Exportoption für benutzerdefinierte Eigenschaften festlegen
            saveOptions.CustomPropertiesExport = PdfCustomPropertiesExport.Standard;

            // Arbeitsmappe als PDF speichern
            workbook.Save("PdfCustomPropertiesExportExample.pdf", saveOptions);

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


