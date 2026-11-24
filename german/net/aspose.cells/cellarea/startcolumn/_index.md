---
title: "CellArea.StartColumn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellArea-Feld. Gibt die Startspalte dieses Bereichs zurück oder setzt sie"
type: docs
url: /de/net/aspose.cells/cellarea/startcolumn/
---
## CellArea.StartColumn field

Liest oder setzt die Startspalte dieses Bereichs.

```csharp
public int StartColumn;
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaFieldStartColumnDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Setzen Sie einige Anfangsdaten
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue(10);
            cells["A3"].PutValue(20);

            // Erstellen Sie ein CellArea und setzen Sie dessen StartColumn
            CellArea area = new CellArea();
            area.StartRow = 1;
            area.EndRow = 3;
            area.StartColumn = 0; // Using StartColumn field
            area.EndColumn = 0;

            // Fügen Sie eine neue Spalte ein, indem Sie vorhandene Zellen nach unten verschieben
            cells.InsertRange(area, ShiftType.Down);

            // Überprüfe das Ergebnis
            Console.WriteLine("A1 value: " + cells["A1"].StringValue); // Should be empty
            Console.WriteLine("A2 value: " + cells["A2"].StringValue); // Should be "Header"
            Console.WriteLine("A3 value: " + cells["A3"].IntValue); // Should be 10
        }
    }
}
```

### Siehe auch

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


