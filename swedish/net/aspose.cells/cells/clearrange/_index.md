---
title: "Cells.ClearRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Rensar innehåll och formatering av ett område"
type: docs
url: /sv/net/aspose.cells/cells/clearrange/
---
## ClearRange(CellArea) {#clearrange}

Rensar innehåll och formatering av ett område.

```csharp
public void ClearRange(CellArea range)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| område | CellArea | Område som ska rensas. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodClearRangeWithCellAreaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll celler med exempeldata
            for (int row = 0; row <= 2; row++)
            {
                for (int col = 0; col <= 2; col++)
                {
                    worksheet.Cells[row, col].Value = $"Data_{row}_{col}";
                }
            }

            // Definiera CellArea att rensa (rader 0-2, kolumner 0-2)
            CellArea clearArea = new CellArea();
            clearArea.StartRow = 0;
            clearArea.EndRow = 2;
            clearArea.StartColumn = 0;
            clearArea.EndColumn = 2;

            try
            {
                // Rensa det angivna området
                worksheet.Cells.ClearRange(clearArea);
                Console.WriteLine("Cleared cells in range: Rows 0-2, Columns 0-2");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearRange method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("CellsMethodClearRangeWithCellAreaDemo.xlsx");
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ClearRange(int, int, int, int) {#clearrange_1}

Rensar innehåll och formatering av ett område.

```csharp
public void ClearRange(int startRow, int startColumn, int endRow, int endColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRow | Int32 | Startradindex. |
| startColumn | Int32 | Startkolumnindex. |
| endRow | Int32 | Slutradindex. |
| endColumn | Int32 | Slutkolumnindex. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodClearRangeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Fyll i några testdata
            cells[0, 0].PutValue(1);
            cells[0, 16383].PutValue(2);
            cells[1048575, 0].PutValue(3);
            cells[1048575, 16383].PutValue(4);

            // Rensa hela kalkylbladets område
            cells.ClearRange(0, 0, 1048575, 16383);

            // Spara arbetsboken
            workbook.Save("ClearRangeDemo.xlsx");

            Console.WriteLine("ClearRange demo executed successfully.");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


