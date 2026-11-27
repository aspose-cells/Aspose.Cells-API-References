---
title: "Klass Font"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Font-klass. Inkapslar teckensnittobjektet som används i ett kalkylblad"
type: docs
url: /sv/net/aspose.cells/font/
---
## Font class

Inkapslar teckenobjektet som används i ett kalkylblad.

```csharp
public class Font
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ArgbColor](../../aspose.cells/font/argbcolor/) { get; set; } | Hämtar och anger färgen med ett 32-bitars ARGB‑värde. |
| [CapsType](../../aspose.cells/font/capstype/) { get; set; } | (**Obsolete.**) Hämtar och anger typ av versaler för text. |
| [Charset](../../aspose.cells/font/charset/) { get; set; } | Representerar teckenuppsättningen. |
| [Color](../../aspose.cells/font/color/) { get; set; } | Hämtar eller anger färgen på teckensnittet. |
| [DoubleSize](../../aspose.cells/font/doublesize/) { get; set; } | Hämtar och anger dubbel storlek på teckensnittet. |
| [IsBold](../../aspose.cells/font/isbold/) { get; set; } | Hämtar eller anger ett värde som indikerar om teckensnittet är fetstil. |
| [IsItalic](../../aspose.cells/font/isitalic/) { get; set; } | Hämtar eller anger ett värde som indikerar om teckensnittet är kursivt. |
| [IsNormalizeHeights](../../aspose.cells/font/isnormalizeheights/) { get; set; } | (**Obsolete.**) Anger om normalisering av höjd som ska tillämpas på textsekvensen. |
| [IsStrikeout](../../aspose.cells/font/isstrikeout/) { get; set; } | Hämtar eller anger ett värde som indikerar om teckensnittet har enkel genomstrykning. |
| [IsSubscript](../../aspose.cells/font/issubscript/) { get; set; } | Hämtar eller anger ett värde som indikerar om teckensnittet är nedsänkt. |
| [IsSuperscript](../../aspose.cells/font/issuperscript/) { get; set; } | Hämtar eller anger ett värde som indikerar om teckensnittet är upphöjt. |
| virtual [Name](../../aspose.cells/font/name/) { get; set; } | Hämtar eller anger namnet på `Font`. |
| [SchemeType](../../aspose.cells/font/schemetype/) { get; set; } | Hämtar och anger schematypen för teckensnittet. |
| [ScriptOffset](../../aspose.cells/font/scriptoffset/) { get; set; } | Hämtar och anger skriptförskjutningen, i procentenheter |
| [Size](../../aspose.cells/font/size/) { get; set; } | Hämtar eller anger storleken på teckensnittet. |
| [StrikeType](../../aspose.cells/font/striketype/) { get; set; } | Hämtar slagtyp för texten. |
| [ThemeColor](../../aspose.cells/font/themecolor/) { get; set; } | Hämtar och anger temafärgen. |
| [Underline](../../aspose.cells/font/underline/) { get; set; } | Hämtar eller anger understrykningsstilen för teckensnittet. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Equals](../../aspose.cells/font/equals/#equals)(Font) | Kontrollerar om två teckensnitt är lika. |
| [SetName](../../aspose.cells/font/setname/)(string, FontSchemeType) | Anger namn och schema för teckensnittet. |
| override [ToString](../../aspose.cells/font/tostring/)() | Returnerar en sträng som representerar det aktuella Cell‑objektet. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class FontDemo
    {
        public static void FontExample()
        {
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();

            // Hämtar referensen till det nyligen tillagda kalkylbladet genom att ange dess bladindex
            Worksheet worksheet = workbook.Worksheets[0];

            // Åtkomst till cellen "A1" från kalkylbladet
            Aspose.Cells.Cell cell = worksheet.Cells["A1"];

            // Lägger till ett värde i cellen "A1"
            cell.PutValue("Hello Aspose!");

            // Åtkomst till teckensnittobjektet för cellstilen
            Aspose.Cells.Font font = cell.GetStyle().Font;

            // Ställer in teckensnittets namn till "Times New Roman"
            font.Name = "Times New Roman";

            // Ställer in teckensnittsstorlek till 14
            font.Size = 14;

            // Ställer in teckensnittsfärg till Röd
            font.Color = Color.Red;

            // Ställer in ytterligare teckensnittsegenskaper
            font.IsBold = true;
            font.IsItalic = true;
            font.Underline = FontUnderlineType.Single;
            font.IsStrikeout = false;
            font.IsSuperscript = false;
            font.IsSubscript = false;
            font.Charset = 1;
            font.CapsType = TextCapsType.None;
            font.StrikeType = TextStrikeType.None;
            font.ScriptOffset = 0;
            font.DoubleSize = 14.0;
            font.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);
            font.ArgbColor = Color.Red.ToArgb();
            font.IsNormalizeHeights = false;
            font.SchemeType = FontSchemeType.None;

            // Sparar Excel-filen
            workbook.Save("FontExample.xlsx");
            workbook.Save("FontExample.pdf");
            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


