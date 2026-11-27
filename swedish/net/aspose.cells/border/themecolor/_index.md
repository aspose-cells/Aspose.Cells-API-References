---
title: "Border.ThemeColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Border‑egenskap. Hämtar och anger temafärgen för kanten"
type: docs
url: /sv/net/aspose.cells/border/themecolor/
---
## Border.ThemeColor property

Hämtar och anger temafärgen för kanten.

```csharp
public ThemeColor ThemeColor { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderPropertyThemeColorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Få åtkomst till en cell och hämta dess stil
            Style style = worksheet.Cells["A1"].GetStyle();

            // Ställ in kantens temafärg
            style.Borders[BorderType.BottomBorder].ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

            // Tillämpa stilen på cellen
            worksheet.Cells["A1"].SetStyle(style);

            // Spara arbetsboken
            workbook.Save("BorderThemeColorDemo.xlsx");
        }
    }
}
```

### Se även

* class [ThemeColor](../../themecolor/)
* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


