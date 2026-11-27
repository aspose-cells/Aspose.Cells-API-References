---
title: "Cells.GetGroupedColumnOutlineLevel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Hämtar kolumnens nollbaserade konturnivå"
type: docs
url: /sv/net/aspose.cells/cells/getgroupedcolumnoutlinelevel/
---
## Cells.GetGroupedColumnOutlineLevel method

Hämtar konturnivån (nollbaserad) för kolumnen.

```csharp
public int GetGroupedColumnOutlineLevel(int columnIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | Int32 | Kolumnindexet |

### Returvärde

Konturnivån för kolumnen

### Anmärkningar

Om kolumnen inte är grupperad, returneras noll.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetGroupedColumnOutlineLevelWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gruppera kolumner (de första 3 kolumnerna) utan att dölja dem
            worksheet.Cells.GroupColumns(0, 2, false);
            
            // Hämta konturnivån för den första kolumnen
            int outlineLevel = worksheet.Cells.GetGroupedColumnOutlineLevel(0);
            
            Console.WriteLine("Outline level of column 0: " + outlineLevel);
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


