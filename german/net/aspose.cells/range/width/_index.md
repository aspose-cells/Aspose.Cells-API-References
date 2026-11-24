---
title: "Range.Width"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Eigenschaft. Gibt die Breite eines Bereichs in Punkten zurück"
type: docs
url: /de/net/aspose.cells/range/width/
---
## Range.Width property

Liefert die Breite eines Bereichs in Punkten.

```csharp
public double Width { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Spaltenbreiten festlegen, um die Width-Eigenschaft zu demonstrieren
            worksheet.Cells.SetColumnWidth(1, 20); // Column B width = 20
            worksheet.Cells.SetColumnWidth(2, 30); // Column C width = 30
            
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C4");
            
            // Bereichsbreite anzeigen (Summe der Spaltenbreiten im Bereich)
            Console.WriteLine("Range Width: " + range.Width);
            
            // Einzelne Eigenschaften zur Überprüfung anzeigen
            Console.WriteLine("Range Left Position: " + range.Left);
            Console.WriteLine("Range Top Position: " + range.Top);
            Console.WriteLine("Range Height: " + range.Height);
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


