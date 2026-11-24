---
title: "Range.RowHeight"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Eigenschaft. Setzt oder liest die Höhe der Zeilen in diesem Bereich"
type: docs
url: /de/net/aspose.cells/range/rowheight/
---
## Range.RowHeight property

Setzt oder liefert die Höhe der Zeilen in diesem Bereich

```csharp
public double RowHeight { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyRowHeightDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Setze einige Daten in der ersten Zeile
            worksheet.Cells["A1"].PutValue("This is a test");
            worksheet.Cells["B1"].PutValue("to demonstrate");
            worksheet.Cells["C1"].PutValue("RowHeight property");

            // Erhalte die anfängliche Zeilenhöhe
            double initialHeight = worksheet.Cells.CreateRange("1:1").RowHeight;
            Console.WriteLine("Initial row height: " + initialHeight);

            // Zeile automatisch anpassen
            worksheet.AutoFitRow(0);

            // Erhalte die neue Zeilenhöhe nach automatischer Anpassung
            double newHeight = worksheet.Cells.CreateRange("1:1").RowHeight;
            Console.WriteLine("Row height after auto-fit: " + newHeight);

            // Manuell eine neue Zeilenhöhe festlegen
            worksheet.Cells.CreateRange("1:1").RowHeight = 30;
            Console.WriteLine("Row height after manual set: " + worksheet.Cells.CreateRange("1:1").RowHeight);
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


