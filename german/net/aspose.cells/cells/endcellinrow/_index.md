---
title: "Cells.EndCellInRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Gibt die letzte Zelle in dieser Zeile zurück."
type: docs
url: /de/net/aspose.cells/cells/endcellinrow/
---
## EndCellInRow(int) {#endcellinrow}

Ermittelt die letzte Zelle in dieser Zeile.

```csharp
public Cell EndCellInRow(int rowIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | Int32 | Zeilenindex. |

### Rückgabewert

Zellobjekt.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodEndCellInRowWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Daten in Zeile 5 (0-basierter Index) füllen
            worksheet.Cells[5, 2].PutValue("Data1");
            worksheet.Cells[5, 4].PutValue("Data2");
            worksheet.Cells[5, 6].PutValue("Data3");

            try
            {
                // Rufe EndCellInRow mit Zeilenindex 5 auf
                Cell endCell = worksheet.Cells.EndCellInRow(5);
                
                if (endCell != null)
                {
                    Console.WriteLine($"Last cell in row 5: {endCell.Name}");
                    Console.WriteLine($"Cell value: {endCell.StringValue}");
                }
                else
                {
                    Console.WriteLine("No cells found in row 5");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing EndCellInRow: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("CellsMethodEndCellInRowWithInt32Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## EndCellInRow(int, int, int, int) {#endcellinrow_1}

Ermittelt die letzte Zelle mit dem maximalen Zeilenindex in diesem Bereich.

```csharp
public Cell EndCellInRow(int startRow, int endRow, int startColumn, int endColumn)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | Int32 | Startzeilenindex. |
| endRow | Int32 | Endzeilenindex. |
| startColumn | Int32 | Startspaltenindex. |
| endColumn | Int32 | Endspaltenindex. |

### Rückgabewert

Zellobjekt.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodEndCellInRowWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einige Daten im Arbeitsblatt einfügen
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell_{i}_{j}");
                }
            }

            // Hole die Endzelle in Zeile 3 zwischen Spalten 1 bis 4
            Cell endCell = worksheet.Cells.EndCellInRow(3, 1, 3, 4);

            // Gib die Zeilen- und Spaltenindizes der Endzelle aus
            Console.WriteLine($"End cell in row 3 between columns 1-4 is at: Row {endCell.Row}, Column {endCell.Column}");
        }
    }
}
```

### Siehe auch

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


