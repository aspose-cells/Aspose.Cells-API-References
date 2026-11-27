---
title: "StyleFlag.VerticalAlignment"
second_title: "Aspose.Cells för .NET API‑referens"
description: "StyleFlag-egenskap. Inställning för vertikal justering kommer att tillämpas"
type: docs
url: /sv/net/aspose.cells/styleflag/verticalalignment/
---
## StyleFlag.VerticalAlignment property

Inställningen för vertikal justering kommer att tillämpas.

```csharp
public bool VerticalAlignment { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyVerticalAlignmentDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Skapa en stil med vertikal justering
            Style style = workbook.CreateStyle();
            style.VerticalAlignment = TextAlignmentType.Center;
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.Font.Color = Color.Blue;

            // Skapa stilflagga för att endast tillämpa vertikal justering och teckenfärg
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.VerticalAlignment = true;
            styleFlag.FontColor = true;

            // Tillämpa stilen på den första raden med stilflaggan
            Row row = sheet.Cells.Rows[0];
            row.ApplyStyle(style, styleFlag);

            // Sätt lite text i cellerna för att se effekten
            sheet.Cells["A1"].PutValue("Vertically Centered");
            sheet.Cells["B1"].PutValue("Blue Text");

            // Spara arbetsboken
            workbook.Save("VerticalAlignmentDemo.xlsx");
        }
    }
}
```

### Se även

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


