---
title: "Cells.EndCellInColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Hämtar den sista cellen i den här kolumnen"
type: docs
url: /sv/net/aspose.cells/cells/endcellincolumn/
---
## EndCellInColumn(int) {#endcellincolumn}

Hämtar den sista cellen i den här kolumnen.

```csharp
public Cell EndCellInColumn(int columnIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | Int32 | Kolumnindex. |

### Returvärde

Cellobjekt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodEndCellInColumnWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            worksheet.Cells["A4"].PutValue("Data3");
            worksheet.Cells["B1"].PutValue("Value1");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Hämta den sista cellen i kolumn A (kolumnindex 0)
            Cell lastCell = worksheet.Cells.EndCellInColumn(0);
            
            Console.WriteLine("Last cell in column A: Row " + lastCell.Row + ", Value: " + lastCell.StringValue);

            // Iterera genom alla rader i kolumn A
            for (int row = 0; row <= lastCell.Row; row++)
            {
                Cell cell = worksheet.Cells[row, 0];
                Console.WriteLine("Row " + row + ": " + cell.StringValue);
            }

            // Spara arbetsboken
            workbook.Save("EndCellInColumnDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## EndCellInColumn(int, int, int, int) {#endcellincolumn_1}

Hämtar den sista cellen med högsta kolumnindex i detta område.

```csharp
public Cell EndCellInColumn(int startRow, int endRow, int startColumn, int endColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRow | Int32 | Startradindex. |
| endRow | Int32 | Slutradindex. |
| startColumn | Int32 | Startkolumnindex. |
| endColumn | Int32 | Slutkolumnindex. |

### Returvärde

Cellobjekt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodEndCellInColumnWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i data i kolumn B (index 1)
            worksheet.Cells[0, 1].PutValue("Data 1");
            worksheet.Cells[2, 1].PutValue("Data 2");
            worksheet.Cells[3, 1].PutValue("Data 3");

            try
            {
                // Anropa EndCellInColumn med parametrarna: startRow=0, endRow=5, startColumn=1, endColumn=1
                Cell result = worksheet.Cells.EndCellInColumn(0, 5, 1, 1);

                if (result != null)
                {
                    Console.WriteLine($"Last cell in column B between rows 0-5 is at row {result.Row}, column {result.Column}");
                    // Markera den hittade cellen
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

            // Spara arbetsboken
            workbook.Save("CellsMethodEndCellInColumnWithInt32Int32Int32Int32Demo.xlsx");
        }
    }
}
```

### Se även

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


