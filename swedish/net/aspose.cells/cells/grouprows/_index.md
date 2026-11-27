---
title: "Cells.GroupRows"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Grupperar rader"
type: docs
url: /sv/net/aspose.cells/cells/grouprows/
---
## GroupRows(int, int, bool) {#grouprows_1}

Grupperar rader.

```csharp
public void GroupRows(int firstIndex, int lastIndex, bool isHidden)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstIndex | Int32 | Det första radindexet som ska grupperas. |
| lastIndex | Int32 | Det sista radindexet som ska grupperas. |
| isHidden | Boolean | Anger om de grupperade raderna är dolda. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGroupRowsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Fyll i lite data
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue($"Group {i + 1}");
                for (int j = 1; j <= 5; j++)
                {
                    cells[i, j].PutValue($"Data {j}");
                }
            }

            // Gruppera rader 1 till 5 (0-baserat index) och dölj dem
            cells.GroupRows(1, 5, true);

            // Ställ in sammanfattningsrad under gruppen
            worksheet.Outline.SummaryRowBelow = false;

            // Spara arbetsboken
            workbook.Save("GroupRowsDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GroupRows(int, int) {#grouprows}

Grupperar rader.

```csharp
public void GroupRows(int firstIndex, int lastIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstIndex | Int32 | Det första radindexet som ska grupperas. |
| lastIndex | Int32 | Det sista radindexet som ska grupperas. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGroupRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Fyll i lite exempeldata
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue("Row " + (i + 1));
            }

            // Gruppera rader 2 till 5 (nollbaserat index)
            cells.GroupRows(1, 4);

            // Spara arbetsboken
            workbook.Save("GroupRowsExample.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


