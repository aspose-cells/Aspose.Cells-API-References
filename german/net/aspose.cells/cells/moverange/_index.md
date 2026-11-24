---
title: "Cells.MoveRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Verschiebt den Bereich"
type: docs
url: /de/net/aspose.cells/cells/moverange/
---
## Cells.MoveRange method

Verschiebt den Bereich.

```csharp
public void MoveRange(CellArea sourceArea, int destRow, int destColumn)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceArea | CellArea | Der Bereich, der verschoben werden soll. |
| destRow | Int32 | Die Zielzeile. |
| destColumn | Int32 | Die Zielspalte. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodMoveRangeWithCellAreaInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Werte in Zellen einfügen
            cells["A1"].PutValue("Original");
            cells["B1"].PutValue(100);
            cells["A2"].PutValue("Data");
            cells["B2"].PutValue(200);

            // Definieren Sie den zu verschiebenden Zellbereich (A1:B2)
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 1;
            area.EndColumn = 1;

            // Verschieben Sie den Bereich um 2 Zeilen nach unten und um 3 Spalten nach rechts
            cells.MoveRange(area, 2, 3);

            // Speichere die Arbeitsmappe
            workbook.Save("MoveRangeExample.xlsx");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


