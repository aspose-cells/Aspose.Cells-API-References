---
title: "ThemeColor.ColorType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThemeColor-egenskap. Hämtar och anger tematypen"
type: docs
url: /sv/net/aspose.cells/themecolor/colortype/
---
## ThemeColor.ColorType property

Hämtar och anger tematypen.

```csharp
public ThemeColorType ColorType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThemeColorPropertyColorTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa två temafärger med olika typer
            ThemeColor color1 = new ThemeColor(ThemeColorType.Accent1, 0.5);
            ThemeColor color2 = new ThemeColor(ThemeColorType.Accent2, 0.3);
            
            // Demonstrera ColorType-egenskapen
            Console.WriteLine("Color1 Type: " + color1.ColorType);
            Console.WriteLine("Color2 Type: " + color2.ColorType);
            
            // Applicera temafärger på celler
            Style style1 = workbook.CreateStyle();
            style1.ForegroundThemeColor = color1;
            worksheet.Cells["A1"].SetStyle(style1);
            
            Style style2 = workbook.CreateStyle();
            style2.ForegroundThemeColor = color2;
            worksheet.Cells["A2"].SetStyle(style2);
            
            // Spara arbetsboken
            workbook.Save("ThemeColorDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ThemeColorType](../../themecolortype/)
* class [ThemeColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


