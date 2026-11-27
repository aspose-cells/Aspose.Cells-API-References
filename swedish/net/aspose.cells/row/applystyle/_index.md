---
title: "Row.ApplyStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Row-metod. Tillämpar format för en hel rad"
type: docs
url: /sv/net/aspose.cells/row/applystyle/
---
## Row.ApplyStyle method

Tillämpar format för en hel rad.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | Stil | Stilobjektet som kommer att tillämpas. |
| flagga | StyleFlag | Flaggor som indikerar tillämpade formateringsegenskaper. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ställ in HTML-innehåll i den första cellen
            sheet.Cells[0, 0].HtmlString = @"<font style=""color: #49c131; font-weight: bold;"">Styled </font><font>text</font>";

            // Hämta den första raden och dess stil
            Row row = sheet.Cells.Rows[0];
            Style style = row.GetStyle();
            
            // Ändra stilegenskaper
            style.IsTextWrapped = true;
            style.HorizontalAlignment = TextAlignmentType.Center;

            // Tillämpa stil med specifika flaggor (endast textbrytning kommer att tillämpas)
            row.ApplyStyle(style, new StyleFlag { WrapText = true });

            // Auto-anpassning för demonstration
            sheet.AutoFitRows();
            sheet.AutoFitColumns();

            // Spara arbetsboken
            workbook.Save("RowApplyStyleDemo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


