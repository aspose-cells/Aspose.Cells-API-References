---
title: "Enum StyleModifyFlag"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.StyleModifyFlag enum. De flaggor som indikerar ändringar i stil"
type: docs
url: /sv/net/aspose.cells/stylemodifyflag/
---
## StyleModifyFlag enumeration

Stilens modifieringsflaggor.

```csharp
public enum StyleModifyFlag
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| LeftBorder | `256` | Indikerar om vänster kant har ändrats för stilen. |
| RightBorder | `512` | Indikerar om höger kant har ändrats för stilen. |
| TopBorder | `1024` | Indikerar om överkant har ändrats för stilen. |
| BottomBorder | `2048` | Indikerar om nederkant har ändrats för stilen. |
| DiagonalDownBorder | `4096` | Indikerar om diagonal‑nedåtriktad kant har ändrats för stilen. |
| DiagonalUpBorder | `8192` | Indikerar om diagonal‑uppåtriktad kant har ändrats för stilen. |
| HorizontalBorder | `32` | Indikerar om horisontell kant har ändrats för stilen. Endast för dynamisk stil, såsom villkorsstyrd formatering. |
| VerticalBorder | `64` | Indikerar om vertikal kant har ändrats för stilen. Endast för dynamisk stil, såsom villkorsstyrd formatering. |
| SideBorders | `3840` | Indikerar de fyra sidogränserna: LeftBorder, RightBorder, TopBorder och BottomBorder. |
| Diagonal | `12288` | Indikerar diagonala kanter: DiagonalDownBorder och DiagonalUpBorder. |
| DynamicStyleBorders | `96` | Indikerar kanter för dynamisk stil: HorizontalBorder och VerticalBorder. |
| Borders | `16224` | Indikerar om en eller flera kanter (LeftBorder, RightBorder, TopBorder, BottomBorder, Diagonal, HorizontalBorder, VerticalBorder) har ändrats för stilen. |
| NumberFormat | `16384` | Indikerar om talformat har ändrats. |
| HorizontalAlignment | `32768` | Indikerar om horisontell justering har ändrats. |
| VerticalAlignment | `65536` | Indikerar om vertikal justering har ändrats. |
| Indent | `131072` | Indikerar om indenteringsegenskap har ändrats. |
| Rotation | `262144` | Indikerar om rotationsegenskap har ändrats. |
| WrapText | `524288` | Indikerar om egenskapen för radbrytning av text har ändrats. |
| ShrinkToFit | `1048576` | Indikerar om egenskapen för krympa för att passa har ändrats. |
| TextDirection | `2097152` | Indikerar om egenskapen för textriktning har ändrats. |
| RelativeIndent | `128` | Anger om relative indent‑egenskapen har ändrats för stilen. Endast för dynamisk stil, såsom villkorsstyrd formatering. |
| AlignmentSettings | `4161664` | Anger om en eller flera justeringsrelaterade egenskaper (HorizontalAlignment, VerticalAlignment, Rotation, WrapText, WrapText, Indent, ShrinkToFit, TextDirection, RelativeIndent) har ändrats. |
| Pattern | `4194304` | Anger om mönstret för skuggning har ändrats. |
| ForegroundColor | `8388608` | Anger om förgrundsfärgen har ändrats. |
| BackgroundColor | `16777216` | Anger om bakgrundsfärgen har ändrats. |
| CellShading | `29360128` | Anger om en eller flera skuggningsrelaterade egenskaper (Pattern, ForegroundColor, BackgroundColor) har ändrats. |
| Locked | `67108864` | Anger om låst egenskap har ändrats. |
| HideFormula | `134217728` | Anger om hide formula har ändrats. |
| ProtectionSettings | `201326592` | Anger om en eller flera skyddsrelaterade egenskaper (Locked, HideFormula) har ändrats. |
| FontSize | `1` | Anger om teckenstorlek har ändrats. |
| FontName | `2` | Anger om teckensnittets namn har ändrats. |
| FontColor | `3` | Anger om teckenfärg har ändrats. |
| FontWeight | `4` | Anger om teckenvikt har ändrats. |
| FontItalic | `5` | Anger om kursiv egenskap för teckensnittet har ändrats. |
| FontUnderline | `6` | Anger om understrykningsegenskap för teckensnittet har ändrats. |
| FontStrike | `7` | Anger om genomstruken egenskap för teckensnittet har ändrats. |
| FontScript | `8` | Anger om nedsänkt eller upphöjd egenskap för teckensnittet har ändrats. |
| FontFamily | `9` | Anger om teckensnittsfamilj har ändrats. |
| FontCharset | `10` | Anger om teckensnittets teckenuppsättning har ändrats. |
| FontScheme | `11` | oanvänd. |
| FontDirty | `12` | oanvänd. |
| FontSpellingError | `13` | oanvänd. |
| FontUFillTx | `14` | oanvänd. |
| FontSpacing | `15` | oanvänd. |
| FontKerning | `16` | oanvänd. |
| FontEqualize | `17` | oanvänd. |
| FontCap | `18` | oanvänd. |
| FontVerticalText | `19` |  |
| Font | `31` | Anger om en eller flera egenskaper har ändrats för stilens teckensnitt. |
| All | `234881023` | Alla egenskaper som kan ändras för stilen. |
| None | `0` | Ingen egenskap har specificerats. |

### Anmärkningar

Kombinationer av flera egenskaper definieras för användarens bekvämlighet. Vid kontroll om de har ändrats för en stil anger det returnerade värdet om en eller flera egenskaper i kombinationen har ändrats.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleModifyFlagDemo
    {
        public static void StyleModifyFlagExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange några värden i kalkylbladet
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["A2"].PutValue(123.45);

            // Skapa en ny stil
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.Color = System.Drawing.Color.Blue;
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;

            // Tillämpa stilen på en cell
            worksheet.Cells["A1"].SetStyle(style);

            // Kontrollera vilka stilegenskaper som har ändrats
            bool isFontModified = style.IsModified(StyleModifyFlag.Font);
            bool isFontSizeModified = style.IsModified(StyleModifyFlag.FontSize);
            bool isFontColorModified = style.IsModified(StyleModifyFlag.FontColor);
            bool isHorizontalAlignmentModified = style.IsModified(StyleModifyFlag.HorizontalAlignment);

            // Skriv ut resultaten
            Console.WriteLine("Font Modified: " + isFontModified);
            Console.WriteLine("Font Size Modified: " + isFontSizeModified);
            Console.WriteLine("Font Color Modified: " + isFontColorModified);
            Console.WriteLine("Horizontal Alignment Modified: " + isHorizontalAlignmentModified);

            // Spara arbetsboken
            workbook.Save("StyleModifyFlagExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


