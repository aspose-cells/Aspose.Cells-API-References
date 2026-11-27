---
title: "CellsHelper.CellNameToIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsHelper‑metod. Hämtar cellens rad‑ och kolumnindex enligt dess namn"
type: docs
url: /sv/net/aspose.cells/cellshelper/cellnametoindex/
---
## CellsHelper.CellNameToIndex method

Hämtar cellens rad- och kolumnindex enligt dess namn.

```csharp
public static void CellNameToIndex(string cellName, out int row, out int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellName | String | Cellens namn. |
| row | Int32& | Radindex för utdata |
| column | Int32& | Kolumnindex för utdata |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperMethodCellNameToIndexWithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Initiera variabler för att hålla rad‑ och kolumnindex
            int rowIndex = -1;
            int columnIndex = -1;
            string cellName = "C5";

            try
            {
                // Anropa CellNameToIndex‑metoden för att konvertera cellnamn till rad‑ och kolumnindex
                CellsHelper.CellNameToIndex(cellName, out rowIndex, out columnIndex);

                // Visa resultaten
                Console.WriteLine($"Cell name: {cellName}");
                Console.WriteLine($"Row index: {rowIndex}");
                Console.WriteLine($"Column index: {columnIndex}");

                // Skapa en arbetsbok och demonstrera användning av indexen
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Få åtkomst till cellen med de erhållna indexen
                Cell cell = worksheet.Cells[rowIndex, columnIndex];
                cell.PutValue("Test Value");

                // Spara arbetsboken
                workbook.Save("CellNameToIndexDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing CellNameToIndex method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


