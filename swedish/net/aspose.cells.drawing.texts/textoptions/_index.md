---
title: "Klass TextOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Texts.TextOptions klass. Representerar textalternativen"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textoptions/
---
## TextOptions class

Representerar textalternativen.

```csharp
public class TextOptions : Font
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ArgbColor](../../aspose.cells/font/argbcolor/) { get; set; } | Hämtar och anger färgen med ett 32-bitars ARGB-värde.(Ärvd från [`Font`](../../aspose.cells/font/).) |
| [CapsType](../../aspose.cells.drawing.texts/textoptions/capstype/) { get; set; } | Hämtar och anger versaltyp för texter i formen. |
| [Charset](../../aspose.cells/font/charset/) { get; set; } | Representerar teckenuppsättningen.(Ärvd från [`Font`](../../aspose.cells/font/).) |
| [Color](../../aspose.cells/font/color/) { get; set; } | Hämtar eller anger Color på teckensnittet.(Ärvd från [`Font`](../../aspose.cells/font/).) |
| [DoubleSize](../../aspose.cells/font/doublesize/) { get; set; } | Hämtar och anger dubbel storlek på teckensnittet.(Ärvd från [`Font`](../../aspose.cells/font/).) |
| [FarEastName](../../aspose.cells.drawing.texts/textoptions/fareastname/) { get; set; } | Hämtar och anger FarEast-namnet. |
| [Fill](../../aspose.cells.drawing.texts/textoptions/fill/) { get; } | Representerar fyllningsformatet för texten. |
| [IsBold](../../aspose.cells/font/isbold/) { get; set; } | Hämtar eller anger ett värde som indikerar om fonten är fetstil.(Ärvd från [`Font`](../../aspose.cells/font/).) |
| [IsItalic](../../aspose.cells/font/isitalic/) { get; set; } | Hämtar eller anger ett värde som indikerar om fonten är kursiv.(Ärvd från [`Font`](../../aspose.cells/font/).) |
| [IsNormalizeHeights](../../aspose.cells.drawing.texts/textoptions/isnormalizeheights/) { get; set; } | Indikerar om normaliseringen av höjden som ska tillämpas på textkörningen. |
| [IsStrikeout](../../aspose.cells/font/isstrikeout/) { get; set; } | Hämtar eller anger ett värde som indikerar om fonten har enkel genomstrykning.(Ärvd från [`Font`](../../aspose.cells/font/).) |
| [IsSubscript](../../aspose.cells/font/issubscript/) { get; set; } | Hämtar eller anger ett värde som indikerar om teckensnittet är nedsänkt.(Ärvd från [`Font`](../../aspose.cells/font/).) |
| [IsSuperscript](../../aspose.cells/font/issuperscript/) { get; set; } | Hämtar eller anger ett värde som indikerar om teckensnittet är upphöjt.(Ärvd från [`Font`](../../aspose.cells/font/).) |
| [Kerning](../../aspose.cells.drawing.texts/textoptions/kerning/) { get; set; } | Anger den minsta teckensnittsstorleken där teckenavstånd (kerning) kommer att tillämpas för detta textsegment. |
| [LanguageCode](../../aspose.cells.drawing.texts/textoptions/languagecode/) { get; set; } | Hämtar och anger språket för användargränssnittet. |
| [LatinName](../../aspose.cells.drawing.texts/textoptions/latinname/) { get; set; } | Hämtar och anger det latinska namnet. |
| override [Name](../../aspose.cells.drawing.texts/textoptions/name/) { get; set; } | Hämtar och anger namnet på formen. |
| [Outline](../../aspose.cells.drawing.texts/textoptions/outline/) { get; } | Representerar konturformatet för texten. |
| [SchemeType](../../aspose.cells/font/schemetype/) { get; set; } | Hämtar och anger teckensnittets schematyp.(Ärvd från [`Font`](../../aspose.cells/font/).) |
| [ScriptOffset](../../aspose.cells/font/scriptoffset/) { get; set; } | Hämtar och anger skriptförskjutningen, i procentenhet(Ärvd från [`Font`](../../aspose.cells/font/).) |
| [Shadow](../../aspose.cells.drawing.texts/textoptions/shadow/) { get; } | Representerar ett [`ShadowEffect`](../../aspose.cells.drawing/shadoweffect/) objekt som specificerar skuggeffekt för diagrammet eller formen. |
| [Size](../../aspose.cells/font/size/) { get; set; } | Hämtar eller anger teckensnittets storlek.(Ärvd från [`Font`](../../aspose.cells/font/).) |
| [Spacing](../../aspose.cells.drawing.texts/textoptions/spacing/) { get; set; } | Anger avståndet mellan tecken inom ett textsegment. |
| [StrikeType](../../aspose.cells/font/striketype/) { get; set; } | Hämtar typ av genomstrykning för texten.(Ärvd från [`Font`](../../aspose.cells/font/).) |
| [ThemeColor](../../aspose.cells/font/themecolor/) { get; set; } | Hämtar och anger temafärgen.(Ärvd från [`Font`](../../aspose.cells/font/).) |
| [Underline](../../aspose.cells/font/underline/) { get; set; } | Hämtar eller anger teckensnittets understrykningstyp.(Ärvd från [`Font`](../../aspose.cells/font/).) |
| [UnderlineColor](../../aspose.cells.drawing.texts/textoptions/underlinecolor/) { get; set; } | Hämtar eller anger färgen på understrykning. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Equals](../../aspose.cells/font/equals/)(Font) | Kontrollerar om två teckensnitt är lika.(Ärvd från [`Font`](../../aspose.cells/font/).) |
| [SetName](../../aspose.cells/font/setname/)(string, FontSchemeType) | Anger namn och schema för teckensnittet.(Ärvd från [`Font`](../../aspose.cells/font/).) |
| override [ToString](../../aspose.cells/font/tostring/)() | Returnerar en sträng som representerar det aktuella Cell‑objektet.(Ärvd från [`Font`](../../aspose.cells/font/).) |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassTextOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en form i kalkylbladet med alla nödvändiga parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
            
            // Lägg till text i formen och hämta TextOptions
            shape.TextBody.Text = "Sample Text";
            TextOptions textOptions = shape.TextBody[2].TextOptions;
            
            // Ange textalternativ
            textOptions.Fill.SolidFill.Color = System.Drawing.Color.Red;
            textOptions.Fill.SolidFill.Transparency = 0.5;
            
            // Spara arbetsboken
            workbook.Save("TextOptionsDemo.xlsx");
        }
    }
}
```

### Se även

* class [Font](../../aspose.cells/font/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


