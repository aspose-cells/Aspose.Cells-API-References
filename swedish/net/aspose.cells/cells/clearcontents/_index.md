---
title: "Cells.ClearContents"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Rensar innehållet i ett område"
type: docs
url: /sv/net/aspose.cells/cells/clearcontents/
---
## ClearContents(CellArea) {#clearcontents}

Rensar innehållet i ett område.

```csharp
public void ClearContents(CellArea range)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| område | CellArea | Område som ska rensas. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodClearContentsWithCellAreaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Fyll i lite data i ett cellområde
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 2;

            for (int row = area.StartRow; row <= area.EndRow; row++)
            {
                for (int col = area.StartColumn; col <= area.EndColumn; col++)
                {
                    cells[row, col].PutValue($"Data_{row}_{col}");
                }
            }

            Console.WriteLine("Before ClearContents:");
            PrintCellAreaContents(cells, area);

            // Rensa innehållet i cellområdet
            cells.ClearContents(area);

            Console.WriteLine("\nAfter ClearContents:");
            PrintCellAreaContents(cells, area);
        }

        private static void PrintCellAreaContents(Cells cells, CellArea area)
        {
            for (int row = area.StartRow; row <= area.EndRow; row++)
            {
                for (int col = area.StartColumn; col <= area.EndColumn; col++)
                {
                    Console.Write(cells[row, col].StringValue + "\t");
                }
                Console.WriteLine();
            }
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

## ClearContents(int, int, int, int) {#clearcontents_1}

Rensar innehållet i ett område.

```csharp
public void ClearContents(int startRow, int startColumn, int endRow, int endColumn)
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
    public class CellsMethodClearContentsWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Fyll i några celler med värden
            cells[0, 0].PutValue("Value A1");
            cells[0, 1].PutValue("Value B1");
            cells[1, 0].PutValue("Value A2");
            cells[1, 1].PutValue("Value B2");

            // Visa originalvärden
            Console.WriteLine("Before ClearContents:");
            Console.WriteLine("A1: " + cells[0, 0].StringValue);
            Console.WriteLine("B1: " + cells[0, 1].StringValue);
            Console.WriteLine("A2: " + cells[1, 0].StringValue);
            Console.WriteLine("B2: " + cells[1, 1].StringValue);

            // Rensa innehållet i cellerna i intervallet (0,1) till (1,1)
            cells.ClearContents(0, 1, 1, 1);

            // Visa värden efter rensning
            Console.WriteLine("\nAfter ClearContents(0, 1, 1, 1):");
            Console.WriteLine("A1: " + cells[0, 0].StringValue);
            Console.WriteLine("B1: " + cells[0, 1].StringValue);
            Console.WriteLine("A2: " + cells[1, 0].StringValue);
            Console.WriteLine("B2: " + cells[1, 1].StringValue);

            // Spara arbetsboken
            workbook.Save("ClearContentsDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


