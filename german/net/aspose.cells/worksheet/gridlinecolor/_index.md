---
title: "Worksheet.GridlineColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Ruft die Farbe der Rasterlinien ab und legt sie fest"
type: docs
url: /de/net/aspose.cells/worksheet/gridlinecolor/
---
## Worksheet.GridlineColor property

Liest und setzt die Farbe der Rasterlinie

```csharp
public Color GridlineColor { get; set; }
```

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyGridlineColorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Setzen Sie die Rasterlinienfarbe auf Rot
            worksheet.GridlineColor = Color.Red;
            
            // Speichere die Arbeitsmappe
            string outputPath = "GridlineColorDemo.xlsx";
            workbook.Save(outputPath);
            
            Console.WriteLine("Gridline color set to red and saved to: " + outputPath);
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


