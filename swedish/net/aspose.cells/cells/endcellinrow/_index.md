---
title: "Cells.EndCellInRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Hämtar den sista cellen i den här raden"
type: docs
url: /sv/net/aspose.cells/cells/endcellinrow/
---
## EndCellInRow(int) {#endcellinrow}

Hämtar den sista cellen i den här raden.

```csharp
public Cell EndCellInRow(int rowIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | Int32 | Radindex. |

### Returvärde

Cellobjekt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodEndCellInRowWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fyll i data i rad 5 (0-baserat index)
            worksheet.Cells[5, 2].PutValue("Data1");
            worksheet.Cells[5, 4].PutValue("Data2");
            worksheet.Cells[5, 6].PutValue("Data3");

            try
            {
                // Anropa EndCellInRow med radindex 5
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

            // Spara arbetsboken
            workbook.Save("CellsMethodEndCellInRowWithInt32Demo.xlsx");
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

## EndCellInRow(int, int, int, int) {#endcellinrow_1}

Hämtar den sista cellen med högsta radindex i detta område.

```csharp
public Cell EndCellInRow(int startRow, int endRow, int startColumn, int endColumn)
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
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodEndCellInRowWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i lite data i kalkylbladet
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell_{i}_{j}");
                }
            }

            // Hämta slutcellen i rad 3 mellan kolumnerna 1 till 4
            Cell endCell = worksheet.Cells.EndCellInRow(3, 1, 3, 4);

            // Skriv ut slutcellens rad- och kolumnindex
            Console.WriteLine($"End cell in row 3 between columns 1-4 is at: Row {endCell.Row}, Column {endCell.Column}");
        }
    }
}
```

### Se även

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


