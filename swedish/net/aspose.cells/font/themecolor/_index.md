---
title: "Font.ThemeColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Font-egenskap. Hämtar och anger temafärgen"
type: docs
url: /sv/net/aspose.cells/font/themecolor/
---
## Font.ThemeColor property

Hämtar och anger temafärgen.

```csharp
public ThemeColor ThemeColor { get; set; }
```

### Anmärkningar

Om fontfärgen inte är en temafärg, returneras NULL.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyThemeColorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Åtkomst till cell A1 och ange text
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Theme Color Demo");

            // Hämta stil och teckensnitt
            Style style = cell.GetStyle();
            Font font = style.Font;

            // Skapa och ange temafärg
            font.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);

            // Tillämpa stilen på cellen
            cell.SetStyle(style);

            // Spara arbetsboken
            workbook.Save("ThemeColorDemo.xlsx");

            // Verifiera temafärgen
            Font savedFont = worksheet.Cells["A1"].GetStyle().Font;
            Console.WriteLine("ThemeColor Type: " + savedFont.ThemeColor.ColorType);
            Console.WriteLine("ThemeColor Tint: " + savedFont.ThemeColor.Tint);
        }
    }
}
```

### Se även

* class [ThemeColor](../../themecolor/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


