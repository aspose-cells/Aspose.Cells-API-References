---
title: "HtmlSaveOptions.ExportWorkbookProperties"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt an, ob Arbeitsmappeneigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die HTML- oder MHT-Datei in Excel importieren möchten, behalten Sie den Standardwert bei"
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/exportworkbookproperties/
---
## HtmlSaveOptions.ExportWorkbookProperties property

Gibt an, ob Arbeitsmappeneigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die html- oder mht-Datei in excel importieren möchten, belassen Sie bitte den Standardwert.

```csharp
public bool ExportWorkbookProperties { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportWorkbookPropertiesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Fügen Sie der Arbeitsmappe einige Daten hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Setzen Sie Arbeitsmappeneigenschaften
            workbook.BuiltInDocumentProperties.Author = "Test Author";
            workbook.BuiltInDocumentProperties.Title = "Test Title";

            // HTML‑Speicheroptionen erstellen
            HtmlSaveOptions options = new HtmlSaveOptions();
            
            // Demonstrieren Sie ExportWorkbookProperties, indem Sie es auf false setzen
            options.ExportWorkbookProperties = false;
            
            // Speichere die Arbeitsmappe als HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML file saved with ExportWorkbookProperties set to false");
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


