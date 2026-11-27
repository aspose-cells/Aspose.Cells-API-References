---
title: "Cells.ShowGroupDetail"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Expanderar de grupperade raderna/kolumnerna"
type: docs
url: /sv/net/aspose.cells/cells/showgroupdetail/
---
## Cells.ShowGroupDetail method

Expanderar de grupperade raderna/kolumnerna.

```csharp
public void ShowGroupDetail(bool isVertical, int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ärVertikal | Boolean | Sant, expanderar de grupperade raderna. |
| index | Int32 | Rad-/kolumnindexet |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodShowGroupDetailWithBooleanInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i exempeldata i rader 5-7 (nollbaserat index 4-6)
            for (int row = 4; row <= 6; row++)
            {
                worksheet.Cells[row, 0].PutValue($"Row {row + 1}");
            }

            // Gruppera rader 4-6 (Excel-rader 5-7) och kollapsa dem initialt
            worksheet.Cells.GroupRows(4, 6, true);

            try
            {
                // Expandera de grupperade raderna med ShowGroupDetail (isVertical: false för rader, index: 4)
                worksheet.Cells.ShowGroupDetail(false, 4);
                Console.WriteLine("ShowGroupDetail method executed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ShowGroupDetail: {ex.Message}");
            }

            // Spara arbetsboken för att demonstrera effekten
            workbook.Save("ShowGroupDetailWithBooleanInt32Demo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


