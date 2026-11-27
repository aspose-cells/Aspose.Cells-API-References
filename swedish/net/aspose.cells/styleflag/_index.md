---
title: "Klass StyleFlag"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.StyleFlag class. Representerar flaggor som indikerar tillämpade formateringsegenskaper"
type: docs
url: /sv/net/aspose.cells/styleflag/
---
## StyleFlag class

Representerar flaggor som indikerar tillämpade formateringsegenskaper.

```csharp
public class StyleFlag
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [StyleFlag](styleflag/)() | Skapar ett objekt med alla flaggor satta till falskt. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Alignments](../../aspose.cells/styleflag/alignments/) { get; set; } | Justeringinställning kommer att tillämpas. |
| [All](../../aspose.cells/styleflag/all/) { get; set; } | Alla egenskaper kommer att tillämpas. |
| [Borders](../../aspose.cells/styleflag/borders/) { get; set; } | Alla kantinställningar kommer att tillämpas. |
| [BottomBorder](../../aspose.cells/styleflag/bottomborder/) { get; set; } | Inställningar för bottenkant kommer att tillämpas. |
| [CellShading](../../aspose.cells/styleflag/cellshading/) { get; set; } | Inställning för cellskuggning kommer att tillämpas. |
| [DiagonalDownBorder](../../aspose.cells/styleflag/diagonaldownborder/) { get; set; } | Inställningar för diagonal nedåtkant kommer att tillämpas. |
| [DiagonalUpBorder](../../aspose.cells/styleflag/diagonalupborder/) { get; set; } | Inställningar för diagonal uppåtkant kommer att tillämpas. |
| [Font](../../aspose.cells/styleflag/font/) { get; set; } | Teckensnittinställningar kommer att tillämpas. |
| [FontBold](../../aspose.cells/styleflag/fontbold/) { get; set; } | Inställning för fetstil i teckensnittet kommer att tillämpas. |
| [FontColor](../../aspose.cells/styleflag/fontcolor/) { get; set; } | Inställning för teckensnittsfärg kommer att tillämpas. |
| [FontItalic](../../aspose.cells/styleflag/fontitalic/) { get; set; } | Inställning för kursiv i teckensnittet kommer att tillämpas. |
| [FontName](../../aspose.cells/styleflag/fontname/) { get; set; } | Inställning för teckensnittets namn kommer att tillämpas. |
| [FontScript](../../aspose.cells/styleflag/fontscript/) { get; set; } | Inställning för teckensnittsskript kommer att tillämpas. |
| [FontSize](../../aspose.cells/styleflag/fontsize/) { get; set; } | Inställning för teckensnittsstorlek kommer att tillämpas. |
| [FontStrike](../../aspose.cells/styleflag/fontstrike/) { get; set; } | Inställning för genomstrykning i teckensnittet kommer att tillämpas. |
| [FontUnderline](../../aspose.cells/styleflag/fontunderline/) { get; set; } | Inställning för understrykning i teckensnittet kommer att tillämpas. |
| [HideFormula](../../aspose.cells/styleflag/hideformula/) { get; set; } | Inställning för att dölja formel kommer att tillämpas. |
| [HorizontalAlignment](../../aspose.cells/styleflag/horizontalalignment/) { get; set; } | Inställning för horisontell justering kommer att tillämpas. |
| [Indent](../../aspose.cells/styleflag/indent/) { get; set; } | Inställning för indenteringsnivå kommer att tillämpas. |
| [LeftBorder](../../aspose.cells/styleflag/leftborder/) { get; set; } | Inställningar för vänsterkant kommer att tillämpas. |
| [Locked](../../aspose.cells/styleflag/locked/) { get; set; } | Inställning för låst kommer att tillämpas. |
| [NumberFormat](../../aspose.cells/styleflag/numberformat/) { get; set; } | Inställning för talformat kommer att tillämpas. |
| [QuotePrefix](../../aspose.cells/styleflag/quoteprefix/) { get; set; } | Inställning för att dölja formel kommer att tillämpas. |
| [RightBorder](../../aspose.cells/styleflag/rightborder/) { get; set; } | Inställningar för högerkant kommer att tillämpas. |
| [Rotation](../../aspose.cells/styleflag/rotation/) { get; set; } | Rotationsinställning kommer att tillämpas. |
| [ShrinkToFit](../../aspose.cells/styleflag/shrinktofit/) { get; set; } | Inställning för krympa för att passa kommer att tillämpas. |
| [TextDirection](../../aspose.cells/styleflag/textdirection/) { get; set; } | Inställning för textriktning kommer att tillämpas. |
| [TopBorder](../../aspose.cells/styleflag/topborder/) { get; set; } | Inställningarna för övre kantlinje kommer att tillämpas. |
| [VerticalAlignment](../../aspose.cells/styleflag/verticalalignment/) { get; set; } | Inställningen för vertikal justering kommer att tillämpas. |
| [WrapText](../../aspose.cells/styleflag/wraptext/) { get; set; } | Inställningen för radbrytning av text kommer att tillämpas. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagDemo
    {
        public static void StyleFlagExample()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Header 1");
            worksheet.Cells["B1"].PutValue("Header 2");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B3"].PutValue(40);

            // Skapa ett nytt stilobjekt
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            // Skapa ett nytt StyleFlag-objekt
            StyleFlag styleFlag = new StyleFlag
            {
                All = true,
                Font = true,
                FontSize = true,
                FontBold = true,
                CellShading = true
            };

            // Applicera stilen på ett cellområde
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B1");
            range.ApplyStyle(style, styleFlag);

            // Spara arbetsboken
            workbook.Save("StyleFlagExample.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


