---
title: "Cells.UnMerge"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Avslår ett specificerat område av sammanslagna celler"
type: docs
url: /sv/net/aspose.cells/cells/unmerge/
---
## Cells.UnMerge method

Delar upp ett angivet område av sammanslagna celler.

```csharp
public void UnMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstRow | Int32 | Första raden i detta område (nollbaserad) |
| firstColumn | Int32 | Första kolumnen i detta område (nollbaserad) |
| totalRows | Int32 | Antal rader (enbaserad) |
| totalColumns | Int32 | Antal kolumner (enbaserad) |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUnMergeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Slå ihop celler först
            cells.Merge(0, 0, 2, 2);
            
            // Avslå de tidigare sammanslagna cellerna
            cells.UnMerge(0, 0, 2, 2);
            
            // Spara arbetsboken
            workbook.Save("UnMergeDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


