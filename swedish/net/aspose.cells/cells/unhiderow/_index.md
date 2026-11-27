---
title: "Cells.UnhideRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metoden. Visar en rad"
type: docs
url: /sv/net/aspose.cells/cells/unhiderow/
---
## Cells.UnhideRow method

Visar en dold rad.

```csharp
public void UnhideRow(int row, double height)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindex. |
| höjd | Double | Radhöjd. Radvärdet ändras endast när raden är dold och det angivna höjdvärdet är positivt. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUnhideRowWithInt32DoubleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Dölj rad 5
            worksheet.Cells.HideRow(5);
            
            // Visa rad 5 med en höjd på 12,75
            worksheet.Cells.UnhideRow(5, 12.75);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


