---
title: "Cells.UngroupColumns"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Avgrupperar kolumner"
type: docs
url: /sv/net/aspose.cells/cells/ungroupcolumns/
---
## Cells.UngroupColumns method

Avgrupperar kolumner.

```csharp
public void UngroupColumns(int firstIndex, int lastIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstIndex | Int32 | Det första kolumnindexet som ska avgrupperas. |
| lastIndex | Int32 | Det sista kolumnindexet som ska avgrupperas. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUngroupColumnsWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gruppera kolumner först för att demonstrera avgruppering
            worksheet.Cells.GroupColumns(0, 2);

            // Avgruppera kolumner (0 till 2)
            worksheet.Cells.UngroupColumns(0, 2);

            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


