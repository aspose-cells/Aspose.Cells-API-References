---
title: "Row.CopySettings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Row-metod. Kopiera inställningar för raden såsom stil, höjd, synlighet ...etc"
type: docs
url: /sv/net/aspose.cells/row/copysettings/
---
## Row.CopySettings method

Kopierar radinställningar, såsom stil, höjd, synlighet, ...etc.

```csharp
public void CopySettings(Row source, bool checkStyle)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| källa | Row | källraden vars inställningar kommer att kopieras till denna |
| checkStyle | Boolean | om kontroll och samla stil. Gäller endast och behövs när två radobjekt tillhör olika arbetsbok och stilarna för två arbetsböcker är olika. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RowMethodCopySettingsWithRowBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa och formatera källrad
            Row sourceRow = worksheet.Cells.Rows[0];
            Style sourceStyle = workbook.CreateStyle();
            sourceStyle.BackgroundColor = Color.Blue;
            sourceRow.ApplyStyle(sourceStyle, new StyleFlag { All = true });
            sourceRow.Height = 25;
            sourceRow.IsHidden = false;

            // Skapa målrad
            Row targetRow = worksheet.Cells.Rows[1];
            
            // Demonstrera CopySettings med copyStyle=true
            targetRow.CopySettings(sourceRow, true);

            // Verifiera att inställningarna kopierades
            Console.WriteLine($"Target row height: {targetRow.Height}");
            Console.WriteLine($"Target row is hidden: {targetRow.IsHidden}");

            workbook.Save("RowCopySettingsDemo.xlsx");
        }
    }
}
```

### Se även

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


