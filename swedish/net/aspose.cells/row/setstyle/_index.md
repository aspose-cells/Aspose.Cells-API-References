---
title: "Row.SetStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Row-metod. Ställer in stilen för denna rad"
type: docs
url: /sv/net/aspose.cells/row/setstyle/
---
## Row.SetStyle method

Anger stilen för den här raden.

```csharp
public void SetStyle(Style style)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | Stil | stilen som ska användas som standardstil för celler i denna rad. |

### Anmärkningar

Denna metod ställer bara in den angivna stilen som standardstil för denna rad, utan att ändra stilinställningarna för befintliga celler i raden. För att uppdatera stilinställningarna för befintliga celler till den angivna stilen samtidigt, vänligen använd [`ApplyStyle`](../applystyle/)

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RowMethodSetStyleWithStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa och konfigurera en stil
            Style style = workbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.Blue;
            style.ForegroundColor = System.Drawing.Color.Red;
            style.Pattern = BackgroundType.DiagonalStripe;

            // Hämta den första raden och tillämpa stil
            Row row = worksheet.Cells.Rows[0];
            row.SetStyle(style);

            // Spara arbetsboken
            workbook.Save("RowStyleDemo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../../style/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


