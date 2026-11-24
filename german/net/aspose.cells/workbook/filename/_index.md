---
title: "Workbook.FileName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Eigenschaft. Liest und setzt den aktuellen Dateinamen"
type: docs
url: /de/net/aspose.cells/workbook/filename/
---
## Workbook.FileName property

Liest und setzt den aktuellen Dateinamen.

```csharp
public string FileName { get; set; }
```

### Hinweise

Wenn die Datei per Stream geöffnet wird und es externe Formelbezüge gibt, bitte den Dateinamen festlegen.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyFileNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            
            // Dateinamen-Eigenschaft festlegen
            wb.FileName = "SampleWorkbook.xlsx";
            
            // Einige Daten hinzufügen, um die Funktionalität zu demonstrieren
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells["A1"].PutValue("Workbook FileName Demo");
            sheet.Cells["A2"].PutValue("Current FileName:");
            sheet.Cells["B2"].PutValue(wb.FileName);
            
            // Speichere die Arbeitsmappe
            wb.Save(wb.FileName);
            
            Console.WriteLine($"Workbook created with filename: {wb.FileName}");
            
            // Ändern des Dateinamens demonstrieren
            Workbook wb2 = new Workbook();
            wb2.FileName = "ChangedName.xlsx";
            Console.WriteLine($"New workbook filename set to: {wb2.FileName}");
            
            // Verwendung externer Links demonstrieren
            if (wb.Worksheets.ExternalLinks.Count > 0)
            {
                string externalSource = wb.Worksheets.ExternalLinks[0].DataSource;
                wb2.FileName = externalSource;
                Console.WriteLine($"Updated filename to external source: {wb2.FileName}");
            }
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


