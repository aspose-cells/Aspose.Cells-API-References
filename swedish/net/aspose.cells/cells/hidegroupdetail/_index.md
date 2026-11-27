---
title: "Cells.HideGroupDetail"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Kollapsar de grupperade raderna/kolumnerna"
type: docs
url: /sv/net/aspose.cells/cells/hidegroupdetail/
---
## Cells.HideGroupDetail method

Komprimerar de grupperade raderna/kolumnerna.

```csharp
public void HideGroupDetail(bool isVertical, int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ärVertikal | Boolean | Sant, kollapsa de grupperade raderna. |
| index | Int32 | Rad-/kolumnindexet |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideGroupDetailWithBooleanInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gruppera rader och dölj detaljer
            worksheet.Cells.GroupRows(0, 9, false);
            worksheet.Cells.HideGroupDetail(true, 4);
            worksheet.Cells.HideGroupDetail(true, 7);

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


