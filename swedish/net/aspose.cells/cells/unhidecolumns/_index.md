---
title: "Cells.UnhideColumns"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Visa flera kolumner"
type: docs
url: /sv/net/aspose.cells/cells/unhidecolumns/
---
## Cells.UnhideColumns method

Visa flera dolda kolumner.

```csharp
public void UnhideColumns(int column, int totalColumns, double width)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| column | Int32 | Kolumnindex. |
| totalColumns | Int32 | Kolumnnummer |
| bredd | Double | Kolumnbredd. |

### Anmärkningar

Applicerar endast kolumnbredden på de dolda kolumnerna.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodUnhideColumnsWithInt32Int32DoubleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Dölj kolumnerna 1-3 (nollbaserat) initialt
            worksheet.Cells.HideColumns(1, 3);

            try
            {
                // Visa kolumner som börjar på index 1 (andra kolumnen), 3 kolumner breda, sätt bredd till 15,5
                worksheet.Cells.UnhideColumns(1, 3, 15.5);

                // Verifiera visade kolumner genom att kontrollera deras bredd
                Console.WriteLine($"Column 1 width after unhiding: {worksheet.Cells.GetColumnWidth(1)}");
                Console.WriteLine("Columns 1-3 successfully unhidden with specified width");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UnhideColumns: {ex.Message}");
            }

            // Spara den modifierade arbetsboken
            workbook.Save("UnhideColumnsWithWidthDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


