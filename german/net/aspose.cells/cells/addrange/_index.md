---
title: "Cells.AddRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Fügt einen Bereichsobjektverweis zu den Zellen hinzu"
type: docs
url: /de/net/aspose.cells/cells/addrange/
---
## Cells.AddRange method

Fügt einen Bereichsobjektverweis zu Zellen hinzu

```csharp
public void AddRange(Range rangeObject)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rangeObject | Range | Das Bereichsobjekt wird in den Zellen enthalten sein |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodAddRangeWithRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Setze einige Beispieldaten in den Bereich
            cells["A1"].PutValue("A1");
            cells["A2"].PutValue("A2");
            cells["B1"].PutValue("B1");
            cells["B2"].PutValue("B2");

            // Erstelle einen Bereich und füge ihn mit AddRange hinzu
            Aspose.Cells.Range range = cells.CreateRange("A1", "B2");
            cells.AddRange(range);

            // Modifiziere das Arbeitsblatt, um die Bereichserweiterung zu demonstrieren
            cells.InsertRow(1);
            cells.InsertColumn(1);

            Console.WriteLine($"Range now has {range.RowCount} rows and {range.ColumnCount} columns");
        }
    }
}
```

### Siehe auch

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


