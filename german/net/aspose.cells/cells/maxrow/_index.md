---
title: "Cells.MaxRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Eigenschaft. Maximaler Zeilenindex einer Zelle, die Daten oder Stil enthält"
type: docs
url: /de/net/aspose.cells/cells/maxrow/
---
## Cells.MaxRow property

Maximaler Zeilenindex der Zelle, die Daten oder einen Stil enthält.

```csharp
public int MaxRow { get; }
```

### Hinweise

Gibt -1 zurück, wenn es keine Zelle gibt, die Daten oder Stil im Arbeitsblatt enthält. Diese Eigenschaft muss Zellen und Zeilen dynamisch iterieren und prüfen, daher ist sie zeitaufwendig und sollte nicht wiederholt aufgerufen werden, etwa wenn sie direkt als Bedingung in einer Schleife verwendet wird.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxRowDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Fügen Sie einige Beispieldaten hinzu
            cells[0, 0].PutValue("Name");
            cells[0, 1].PutValue("Age");
            cells[1, 0].PutValue("John");
            cells[1, 1].PutValue(30);
            cells[2, 0].PutValue("Alice");
            cells[2, 1].PutValue(25);

            // Hole den maximalen Zeilenindex (nullbasiert)
            int maxRow = cells.MaxRow;
            Console.WriteLine("MaxRow before adding new data: " + maxRow);

            // Füge neue Daten in die nächste Zeile nach der maximalen Zeile ein
            int newRow = maxRow + 1;
            cells[newRow, 0].PutValue("Bob");
            cells[newRow, 1].PutValue(28);

            // Überprüfe die neue maximale Zeile
            Console.WriteLine("MaxRow after adding new data: " + cells.MaxRow);

            // Speichere die Arbeitsmappe
            workbook.Save("MaxRowDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


