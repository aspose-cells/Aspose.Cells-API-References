---
title: "CellArea.CreateCellArea"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellArea-metod. Skapar ett cellområde"
type: docs
url: /sv/net/aspose.cells/cellarea/createcellarea/
---
## CreateCellArea(int, int, int, int) {#createcellarea}

Skapar ett cellområde.

```csharp
public static CellArea CreateCellArea(int startRow, int startColumn, int endRow, int endColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRow | Int32 | Startraden. |
| startColumn | Int32 | Startkolumnen. |
| endRow | Int32 | Slutrad. |
| endColumn | Int32 | Slutkolumn. |

### Returvärde

Returnera ett [`CellArea`](../).

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaMethodCreateCellAreaWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Fyll celler med exempeldata
            int[] values = { 1, 3, 2, 6, 4, 5, 8, 9, 7 };
            for (int i = 0; i < values.Length; i++)
            {
                cells[i, i / 3].PutValue(values[i]);
            }

            // Skapa och konfigurera datasortering
            DataSorter sorter = wb.DataSorter;
            sorter.Clear();
            sorter.Order1 = SortOrder.Ascending;
            sorter.Key1 = 2;
            sorter.Order2 = SortOrder.Ascending;
            sorter.Key2 = 1;
            sorter.Order3 = SortOrder.Ascending;
            sorter.Key3 = 0;

            // Sortera med CreateCellArea och Int32-parametrar
            sorter.Sort(cells, CellArea.CreateCellArea(0, 0, 8, 2));

            // Skriv ut sorterade värden
            Console.WriteLine("Sorted values:");
            for (int i = 0; i < 9; i++)
            {
                Console.WriteLine(cells[i, 2 - i / 3].IntValue);
            }
        }
    }
}
```

### Se även

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateCellArea(string, string) {#createcellarea_1}

Skapar ett cellområde.

```csharp
public static CellArea CreateCellArea(string startCellName, string endCellName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startCellName | String | Den övre vänstra cellen i området. |
| endCellName | String | Den nedre högra cellen i området. |

### Returvärde

Returnera ett [`CellArea`](../).

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaMethodCreateCellAreaWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Fyll i viss data i kolumn A
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue($"Data {i}");
            }

            // Skapa cellområde från B1 till B10
            CellArea area = CellArea.CreateCellArea("B1", "B10");
            
            // Infoga område som flyttar celler nedåt
            cells.InsertRange(area, ShiftType.Down);
            
            // Verifiera operationen genom att kontrollera cellvärden
            Console.WriteLine("Inserted range from B1 to B10. Total rows: " + cells.Rows.Count);
        }
    }
}
```

### Se även

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


