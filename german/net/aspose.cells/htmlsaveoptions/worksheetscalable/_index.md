---
title: "HtmlSaveOptions.WorksheetScalable"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt an, ob beim Speichern einer Datei als HTML über das Arbeitsblatt-Zoom-Level gezoomt wird. Der Standardwert ist false."
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/worksheetscalable/
---
## HtmlSaveOptions.WorksheetScalable property

Gibt an, ob beim Speichern der Datei nach HTML über die Arbeitsblatt‑Zoomstufe in die HTML gezoomt wird. Der Standardwert ist false.

```csharp
public bool WorksheetScalable { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyWorksheetScalableDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // HTML-Speicheroptionen mit der WorksheetScalable-Eigenschaft festlegen
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.WorksheetScalable = true;
            
            // Speichere die Arbeitsmappe mit HTML-Optionen
            string outputPath = "output.html";
            workbook.Save(outputPath, options);
            
            // Überprüfen, ob die Ausgabe den Skalierungsstil enthält
            string htmlContent = File.ReadAllText(outputPath);
            Console.WriteLine("HTML contains scaling: " + htmlContent.Contains("transform: scale"));
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


