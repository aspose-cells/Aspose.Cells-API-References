---
title: "Cells.HideColumns"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells‑metod. Dölj flera kolumner"
type: docs
url: /sv/net/aspose.cells/cells/hidecolumns/
---
## Cells.HideColumns method

Dölj flera kolumner.

```csharp
public void HideColumns(int column, int totalColumns)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| column | Int32 | Kolumnindex. |
| totalColumns | Int32 | Kolumnnummer. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideColumnsWithInt32Int32Demo
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
                for (int j = 0; j < 10; j++)
                {
                    cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Dölj kolumnerna 3 till 5 (nollbaserat index)
            int startColumn = 2; // Column C
            int columnCount = 3;  // Hide 3 columns
            cells.HideColumns(startColumn, columnCount);

            // Spara arbetsboken
            workbook.Save("HideColumnsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


