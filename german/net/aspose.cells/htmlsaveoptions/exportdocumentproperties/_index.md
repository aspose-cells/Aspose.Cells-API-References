---
title: "HtmlSaveOptions.ExportDocumentProperties"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt an, ob Dokumenteigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die HTML- oder MHT-Datei nach Excel importieren möchten, behalten Sie bitte den Standardwert bei."
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/exportdocumentproperties/
---
## HtmlSaveOptions.ExportDocumentProperties property

Gibt an, ob Dokumenteigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die html- oder mht-Datei in excel importieren möchten, belassen Sie bitte den Standardwert.

```csharp
public bool ExportDocumentProperties { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge einige Dokumenteigenschaften hinzu
            workbook.BuiltInDocumentProperties.Author = "Test Author";
            workbook.BuiltInDocumentProperties.Title = "Test Document";
            
            // Füge Beispieldaten für Zellen hinzu
            worksheet.Cells["A1"].PutValue("Sample HTML Export");
            
            // Erstelle HTML-Speicheroptionen und setze ExportDocumentProperties auf false
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportDocumentProperties = false;
            
            // Speichere die Arbeitsmappe als HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML file saved with document properties export disabled.");
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


