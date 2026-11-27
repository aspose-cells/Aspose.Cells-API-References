---
title: "Cells.SetColumnWidth"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metoden. Ställer in bredden på den angivna kolumnen i normal vy"
type: docs
url: /sv/net/aspose.cells/cells/setcolumnwidth/
---
## Cells.SetColumnWidth method

Ställer in bredden på den angivna kolumnen i normal vy.

```csharp
public void SetColumnWidth(int column, double width)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| column | Int32 | Kolumnindex. |
| bredd | Double | Kolumnbredd i teckenenheter. Kolumnbredden måste vara mellan 0 och 255. |

### Anmärkningar

För kalkylblad mäts kolumnbredden som antalet tecken av den maximala siffrabredden för siffrorna 0~9 när de visas i normalstilens teckensnitt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetColumnWidthWithInt32DoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells.SetColumnWidth(0, 25.5);
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


