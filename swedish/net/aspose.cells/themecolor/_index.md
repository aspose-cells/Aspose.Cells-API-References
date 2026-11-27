---
title: "Klass ThemeColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ThemeColor klass. Representerar en temafärg"
type: docs
url: /sv/net/aspose.cells/themecolor/
---
## ThemeColor class

Representerar en temafärg.

```csharp
public class ThemeColor
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [ThemeColor](themecolor/)(ThemeColorType, double) |  |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ColorType](../../aspose.cells/themecolor/colortype/) { get; set; } | Hämtar och anger tematypen. |
| [Tint](../../aspose.cells/themecolor/tint/) { get; set; } | Hämtar och anger nyansvärdet. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThemeColorDemo
    {
        public static void ThemeColorExample()
        {
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Lägger till ett värde i cell A1
            cells["A1"].PutValue("Hello World");

            // Hämtar stilen för cell A1
            Style style = cells["A1"].GetStyle();

            // Ställ in färgtypen ThemeColorType.Text2 med 40 % ljusare som teckensnittsfärg.
            style.Font.ThemeColor = new ThemeColor(ThemeColorType.Text2, 0.4);
            style.Pattern = BackgroundType.Solid;

            // Ställ in färgtypen ThemeColorType.Background2 med 75 % mörkare som förgrundsfärg
            style.ForegroundThemeColor = new ThemeColor(ThemeColorType.Background2, -0.75);

            // Tillämpar stilen på cell A1
            cells["A1"].SetStyle(style);

            // Sparar Excel-filen
            workbook.Save("ThemeColorExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


