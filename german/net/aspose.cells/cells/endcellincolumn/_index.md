---
title: "Cells.EndCellInColumn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Gibt die letzte Zelle in dieser Spalte zurück"
type: docs
url: /de/net/aspose.cells/cells/endcellincolumn/
---
## EndCellInColumn(int) {#endcellincolumn}

Ermittelt die letzte Zelle in dieser Spalte.

```csharp
public Cell EndCellInColumn(int columnIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | Int32 | Spaltenindex. |

### Rückgabewert

Zellobjekt.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodEndCellInColumnWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            worksheet.Cells["A4"].PutValue("Data3");
            worksheet.Cells["B1"].PutValue("Value1");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Erhalte die letzte Zelle in Spalte A (Spaltenindex 0)
            Cell lastCell = worksheet.Cells.EndCellInColumn(0);
            
            Console.WriteLine("Last cell in column A: Row " + lastCell.Row + ", Value: " + lastCell.StringValue);

            // Iteriere über alle Zeilen in Spalte A
            for (int row = 0; row <= lastCell.Row; row++)
            {
                Cell cell = worksheet.Cells[row, 0];
                Console.WriteLine("Row " + row + ": " + cell.StringValue);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("EndCellInColumnDemo.xlsx");
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

## EndCellInColumn(int, int, int, int) {#endcellincolumn_1}

Ermittelt die letzte Zelle mit dem maximalen Spaltenindex in diesem Bereich.

```csharp
public Cell EndCellInColumn(int startRow, int endRow, int startColumn, int endColumn)
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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodEndCellInColumnWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fülle Daten in Spalte B (Index 1)
            worksheet.Cells[0, 1].PutValue("Data 1");
            worksheet.Cells[2, 1].PutValue("Data 2");
            worksheet.Cells[3, 1].PutValue("Data 3");

            try
            {
                // Rufe EndCellInColumn mit den Parametern auf: startRow=0, endRow=5, startColumn=1, endColumn=1
                Cell result = worksheet.Cells.EndCellInColumn(0, 5, 1, 1);

                if (result != null)
                {
                    Console.WriteLine($"Last cell in column B between rows 0-5 is at row {result.Row}, column {result.Column}");
                    // Markiere die gefundene Zelle
                    result.PutValue("Last Cell");
                    Style style = result.GetStyle();
                    style.Font.IsBold = true;
                    result.SetStyle(style);
                }
                else
                {
                    Console.WriteLine("No cells found in specified range");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing EndCellInColumn method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("CellsMethodEndCellInColumnWithInt32Int32Int32Int32Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


