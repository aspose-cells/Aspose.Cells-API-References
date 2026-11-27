---
title: "Cells.SetColumnWidthPixel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Anger kolumnbredd i enheten pixlar i normal vy"
type: docs
url: /sv/net/aspose.cells/cells/setcolumnwidthpixel/
---
## Cells.SetColumnWidthPixel method

Ställer in kolumnbredd i enhet pixlar i normal vy.

```csharp
public void SetColumnWidthPixel(int column, int pixels)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| column | Int32 | Kolumnindex. |
| pixlar | Int32 | Antal pixlar. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetColumnWidthPixelWithInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ställ in kolumnbredder i pixlar för kolumnerna 1 till 5
            for (int i = 0; i < 5; i++)
            {
                cells.SetColumnWidthPixel(i, 120); // 120 pixels width
            }

            // Spara arbetsboken
            workbook.Save("SetColumnWidthPixelDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


