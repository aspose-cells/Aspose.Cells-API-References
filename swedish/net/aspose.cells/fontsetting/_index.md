---
title: "Klass FontSetting"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.FontSetting-klass. Representerar ett intervall av tecken inom celltexten"
type: docs
url: /sv/net/aspose.cells/fontsetting/
---
## FontSetting class

Representerar ett intervall av tecken inom celltexten.

```csharp
public class FontSetting
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [FontSetting](fontsetting/)(int, int, WorksheetCollection) |  |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Returnerar teckensnittet för detta objekt. |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Hämtar längden på tecknen. |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Hämtar startindexet för tecknen. |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Returnerar textalternativen. |
| virtual [Type](../../aspose.cells/fontsetting/type/) { get; } | Hämtar typen av textnod. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | Ställer in den förinställda WordArt-stilen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class FontSettingDemo
    {
        public static void FontSettingExample()
        {
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();

            // Lägger till ett nytt kalkylblad i Excel-objektet
            workbook.Worksheets.Add();

            // Hämtar referensen till det nyligen tillagda kalkylbladet genom att ange dess bladindex
            Worksheet worksheet = workbook.Worksheets[0];

            // Åtkomst till cellen "A1" från kalkylbladet
            Aspose.Cells.Cell cell = worksheet.Cells["A1"];

            // Lägger till ett värde i cellen "A1"
            cell.PutValue("Visit Aspose!");

            // Hämtar teckenintervall
            FontSetting character = cell.Characters(6, 7);

            // Ställer in teckensnittet för markerade tecken till fetstil
            character.Font.IsBold = true;

            // Ställer in teckenfärgen för markerade tecken till blå
            character.Font.Color = Color.Blue;

            // Sparar Excel-filen
            workbook.Save("FontSettingExample.xlsx");
            workbook.Save("FontSettingExample.pdf");

        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


