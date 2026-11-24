---
title: "AutoFitterOptions.IgnoreHidden"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AutoFitterOptions-Eigenschaft. Ignoriert versteckte Zeilen/Spalten"
type: docs
url: /de/net/aspose.cells/autofitteroptions/ignorehidden/
---
## AutoFitterOptions.IgnoreHidden property

Ignoriert die ausgeblendeten Zeilen/Spalten.

```csharp
public bool IgnoreHidden { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyIgnoreHiddenDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten festlegen und Zeilen formatieren
            worksheet.Cells["A1"].PutValue("This is a test string for autofit");
            worksheet.Cells["A2"].PutValue("Another test string");
            
            // Zeile 1 ausblenden
            worksheet.Cells.Rows[1].IsHidden = true;

            // Erstelle AutoFitterOptions mit IgnoreHidden auf true gesetzt
            AutoFitterOptions options = new AutoFitterOptions
            {
                IgnoreHidden = true,
                AutoFitMergedCells = false,
                OnlyAuto = false
            };

            // Zeilen automatisch anpassen, während versteckte Zeilen ignoriert werden
            worksheet.AutoFitRows(options);

            // Gib die Zeilenhöhen aus
            Console.WriteLine("Row 0 height: " + worksheet.Cells.GetRowHeight(0));
            Console.WriteLine("Row 1 height: " + worksheet.Cells.GetRowHeight(1));
        }
    }
}
```

### Siehe auch

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


