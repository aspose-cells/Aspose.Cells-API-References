---
title: "Cells.MinDataColumn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Eigenschaft. Minimaler Spaltenindex einer Zelle, die Daten enthält"
type: docs
url: /de/net/aspose.cells/cells/mindatacolumn/
---
## Cells.MinDataColumn property

Minimaler Spaltenindex der Zelle, die Daten enthält.

```csharp
public int MinDataColumn { get; }
```

### Hinweise

-1 will be returned if there is no cell which contains data. This property needs to iterate and check all cells in a worksheet dynamically, so it is a time-consumed progress and should not be invoked repeatedly, such as using it directly as condition in a loop.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMinDataColumnDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Fügen Sie einige Daten zu Zellen hinzu (beginnend bei Spalte 2)
            cells["B1"].PutValue("Header1");
            cells["C2"].PutValue("Data1");
            cells["D3"].PutValue("Data2");
            cells["E4"].PutValue("Data3");
            
            // Ermitteln Sie den minimalen Spaltenindex, der Daten enthält
            int minDataColumn = cells.MinDataColumn;
            
            // Gib das Ergebnis aus
            Console.WriteLine("Minimum data column index: " + minDataColumn);
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


