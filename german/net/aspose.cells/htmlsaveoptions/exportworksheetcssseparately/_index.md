---
title: "HtmlSaveOptions.ExportWorksheetCSSSeparately"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt an, ob das Arbeitsblatt‑CSS separat exportiert wird. Der Standardwert ist false."
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/exportworksheetcssseparately/
---
## HtmlSaveOptions.ExportWorksheetCSSSeparately property

Gibt an, ob das CSS des Worksheets separat exportiert wird. Der Standardwert ist false.

```csharp
public bool ExportWorksheetCSSSeparately { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportWorksheetCSSSeparatelyDemo
    {
        public static void Run()
        {
            // Erstelle eine Beispielarbeitsmappe mit Testdaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");
            
            // Setzen Sie HTML-Speicheroptionen mit ExportWorksheetCSSSeparately
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportWorksheetCSSSeparately = true;
            
            // Speichere die Arbeitsmappe als HTML
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "output.html");
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("HTML file with separate CSS saved to: " + outputPath);
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


