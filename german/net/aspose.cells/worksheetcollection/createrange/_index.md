---
title: "WorksheetCollection.CreateRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorksheetCollection-Methode. Erstellt ein Range-Objekt aus einer Adresse des Bereichs"
type: docs
url: /de/net/aspose.cells/worksheetcollection/createrange/
---
## WorksheetCollection.CreateRange method

Erstellt ein [`Range`](../../range/) Objekt aus einer Adresse des Bereichs.

```csharp
public Range CreateRange(string address, int sheetIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| address | String | Die Adresse des Bereichs. |
| sheetIndex | Int32 | Der Blattindex. |

### Rückgabewert

Ein [`Range`](../../range/) Objekt

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodCreateRangeWithStringInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einige Beispieldaten einfügen
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 6; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell {i+1},{j+1}");
                }
            }

            // Erstelle einen Bereich mithilfe einer Zeichenkettenadresse und des Tabellenblatt-Index
            Aspose.Cells.Range range = workbook.Worksheets.CreateRange("A1:F10", 0);

            // Demonstriere die Verwendung des Bereichs
            Console.WriteLine($"Range has {range.RowCount} rows and {range.ColumnCount} columns");
            Console.WriteLine($"First cell value: {range[0, 0].StringValue}");
            Console.WriteLine($"Last cell value: {range[9, 5].StringValue}");
        }
    }
}
```

### Siehe auch

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


