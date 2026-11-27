---
title: "Klass TextParagraph"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Texts.TextParagraph-klass. Representerar textparagrafinställningen"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textparagraph/
---
## TextParagraph class

Representerar inställningen för textstycke.

```csharp
public class TextParagraph : FontSetting
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AlignmentType](../../aspose.cells.drawing.texts/textparagraph/alignmenttype/) { get; set; } | Hämtar och sätter den horisontella justeringstypen för texten i paragrafen. |
| [Bullet](../../aspose.cells.drawing.texts/textparagraph/bullet/) { get; } | Hämtar punkttecknet. |
| [Children](../../aspose.cells.drawing.texts/textparagraph/children/) { get; } | Hämtar alla textkörningar i denna paragraf. Om paragrafen är tom, returneras paragrafen själv. |
| [DefaultTabSize](../../aspose.cells.drawing.texts/textparagraph/defaulttabsize/) { get; set; } | Hämtar och sätter standardstorleken för ett tabulatortecken i denna paragraf. |
| [FirstLineIndent](../../aspose.cells.drawing.texts/textparagraph/firstlineindent/) { get; set; } | Anger indenteringsstorleken som ska tillämpas på den första textraden i paragrafen. |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Returnerar teckensnittet för detta objekt. (Ärvt från [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [FontAlignType](../../aspose.cells.drawing.texts/textparagraph/fontaligntype/) { get; set; } | Bestämmer var vertikalt på en textrad de faktiska orden placeras. Detta hanterar vertikal placering av tecknen i förhållande till baslinjerna. |
| [IsEastAsianLineBreak](../../aspose.cells.drawing.texts/textparagraph/iseastasianlinebreak/) { get; set; } | Anger om ett östasiatiskt ord kan brytas i två delar och radbrytas till nästa rad utan att ett bindestreck läggs till. |
| [IsHangingPunctuation](../../aspose.cells.drawing.texts/textparagraph/ishangingpunctuation/) { get; set; } | Anger om interpunktion ska tvingas placeras på samma rad som texten eller sättas på en annan rad. |
| [IsLatinLineBreak](../../aspose.cells.drawing.texts/textparagraph/islatinlinebreak/) { get; set; } | Anger om ett latinskt ord kan brytas i två delar och radbrytas till nästa rad utan att ett bindestreck läggs till. |
| [LeftMargin](../../aspose.cells.drawing.texts/textparagraph/leftmargin/) { get; set; } | Anger vänstermarginalen för paragrafen. |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Hämtar längden på tecknen. (Ärvt från [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [LineSpace](../../aspose.cells.drawing.texts/textparagraph/linespace/) { get; set; } | Hämtar och sätter mängden vertikalt blankutrymme som ska användas inom en paragraf. |
| [LineSpaceSizeType](../../aspose.cells.drawing.texts/textparagraph/linespacesizetype/) { get; set; } | Hämtar och sätter mängden vertikalt blankutrymme som ska användas inom en paragraf. |
| [RightMargin](../../aspose.cells.drawing.texts/textparagraph/rightmargin/) { get; set; } | Anger högermarginalen för paragrafen. |
| [SpaceAfter](../../aspose.cells.drawing.texts/textparagraph/spaceafter/) { get; set; } | Hämtar och sätter mängden vertikalt blankutrymme som kommer att finnas efter en paragraf. |
| [SpaceAfterSizeType](../../aspose.cells.drawing.texts/textparagraph/spaceaftersizetype/) { get; set; } | Hämtar och sätter mängden vertikalt blankutrymme som kommer att finnas efter en paragraf. |
| [SpaceBefore](../../aspose.cells.drawing.texts/textparagraph/spacebefore/) { get; set; } | Hämtar och sätter mängden vertikalt blankutrymme som kommer att finnas före en paragraf. |
| [SpaceBeforeSizeType](../../aspose.cells.drawing.texts/textparagraph/spacebeforesizetype/) { get; set; } | Hämtar och sätter mängden vertikalt blankutrymme som kommer att finnas före en paragraf. |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Hämtar startindexet för tecknen. (Ärvt från [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [Stops](../../aspose.cells.drawing.texts/textparagraph/stops/) { get; } | Hämtar tabbstopp-listan. |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Returnerar textalternativen. (Ärvt från [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.texts/textparagraph/type/) { get; } | Hämtar typen av textnod. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | Ställer in den förinställda WordArt‑stilen. (Ärvt från [`FontSetting`](../../aspose.cells/fontsetting/).) |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassTextParagraphDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till en textruta i kalkylbladet
            int textBoxIndex = sheet.TextBoxes.Add(10, 10, 200, 100);
            Aspose.Cells.Drawing.TextBox textBox = sheet.TextBoxes[textBoxIndex];
            
            // Ange textinnehåll med flera stycken
            textBox.Text = "First paragraph\nSecond paragraph\nThird paragraph";

            // Åtkomst till och ändring av textparagrafer
            foreach (TextParagraph paragraph in textBox.TextBody.TextParagraphs)
            {
                // Ställ in paragrafegenskaper
                paragraph.LineSpaceSizeType = LineSpaceSizeType.Points;
                paragraph.LineSpace = 20;
                paragraph.AlignmentType = TextAlignmentType.Center;
            }

            // Spara arbetsboken
            workbook.Save("TextParagraphDemo.xlsx");
        }
    }
}
```

### Se även

* class [FontSetting](../../aspose.cells/fontsetting/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


