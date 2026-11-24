---
title: "HtmlSaveOptions.ExportBogusRowData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt an, ob gefälschte Daten der unteren Zeile exportiert werden. Der Standardwert ist true. Wenn Sie die HTML- oder MHT-Datei in Excel importieren möchten, behalten Sie bitte den Standardwert bei."
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/exportbogusrowdata/
---
## HtmlSaveOptions.ExportBogusRowData property

Gibt an, ob gefälschte Daten in der unteren Zeile exportiert werden. Der Standardwert ist true. Wenn Sie die html- oder mht-Datei in excel importieren möchten, belassen Sie bitte den Standardwert.

```csharp
public bool ExportBogusRowData { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportBogusRowDataDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Einige Daten zu den Zellen hinzufügen
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // HTML‑Speicheroptionen erstellen
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            
            // Erster Export ohne gefälschte Zeilendaten
            saveOptions.ExportBogusRowData = false;
            workbook.Save("output_without_bogus.html", saveOptions);
            
            // Dann Export mit gefälschten Zeilendaten
            saveOptions.ExportBogusRowData = true;
            workbook.Save("output_with_bogus.html", saveOptions);

            // Ergebnisse anzeigen
            Console.WriteLine("HTML files created successfully.");
            Console.WriteLine("Check output_without_bogus.html and output_with_bogus.html to see the difference.");
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


