---
title: "Cells.UngroupRows"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Avgrupperar rader"
type: docs
url: /sv/net/aspose.cells/cells/ungrouprows/
---
## UngroupRows(int, int, bool) {#ungrouprows_1}

Avgrupperar rader.

```csharp
public void UngroupRows(int firstIndex, int lastIndex, bool isAll)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstIndex | Int32 | Det första radindexet som ska avgrupperas. |
| lastIndex | Int32 | Det sista radindexet som ska avgrupperas. |
| isAll | Boolean | Sant, tar bort all grupperad information. Annars tas den yttre gruppinformationen bort. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodUngroupRowsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa nästlade radgrupperingar för demonstration
            worksheet.Cells.GroupRows(5, 7);  // First level grouping
            worksheet.Cells.GroupRows(5, 7);  // Second level grouping

            try
            {
                // Avgruppa alla nivåer av rader 5-7
                worksheet.Cells.UngroupRows(5, 7, true);

                Console.WriteLine("Rows 5-7 successfully ungrouped with all levels removed");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UngroupRows: {ex.Message}");
            }

            // Spara den modifierade arbetsboken
            workbook.Save("UngroupRowsWithBooleanDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## UngroupRows(int, int) {#ungrouprows}

Avgrupperar rader.

```csharp
public void UngroupRows(int firstIndex, int lastIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstIndex | Int32 | Det första radindexet som ska avgrupperas. |
| lastIndex | Int32 | Det sista radindexet som ska avgrupperas. |

### Anmärkningar

Tar bara bort yttre gruppinformation.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUngroupRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Fyll i lite data
            for (int i = 0; i < 6; i++)
            {
                cells[i, 0].PutValue($"Row {i}");
            }

            // Gruppera rader 1 till 3 (0-baserat index)
            cells.GroupRows(1, 3, true);

            Console.WriteLine("Rows grouped from index 1 to 3");

            // Avgruppa samma rader
            cells.UngroupRows(1, 3);

            Console.WriteLine("Rows ungrouped from index 1 to 3");

            // Spara arbetsboken
            workbook.Save("UngroupRowsDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


