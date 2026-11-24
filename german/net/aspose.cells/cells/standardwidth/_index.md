---
title: "Cells.StandardWidth"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Eigenschaft. Gibt die Standardspaltenbreite im Arbeitsblatt in Zeichen zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells/cells/standardwidth/
---
## Cells.StandardWidth property

Liest oder setzt die Standardspaltenbreite im Arbeitsblatt, in Zeichen.

```csharp
public double StandardWidth { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardWidthDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Setze die Standardbreite für Spalten
            cells.StandardWidth = 18.25;

            // Zeige die Standardbreite und die tatsächliche Breite der ersten Spalte an
            Console.WriteLine("Standard Width: " + cells.StandardWidth);
            Console.WriteLine("Column 0 Width: " + cells.GetColumnWidth(0));

            // Überprüfe, dass die Standardbreite (ungefähr) angewendet wurde
            if (Math.Abs(cells.GetColumnWidth(0) - cells.StandardWidth) > 1.0)
            {
                Console.WriteLine("Warning: Column width differs significantly from standard width");
            }
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


