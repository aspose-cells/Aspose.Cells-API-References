---
title: "Cells.HideRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Döljer en rad"
type: docs
url: /sv/net/aspose.cells/cells/hiderow/
---
## Cells.HideRow method

Döljer en rad.

```csharp
public void HideRow(int row)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindex. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideRowWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Dölj rad 5
            worksheet.Cells.HideRow(5);
            
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


