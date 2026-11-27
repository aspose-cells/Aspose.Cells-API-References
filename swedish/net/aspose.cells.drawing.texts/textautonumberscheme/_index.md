---
title: "Enum TextAutonumberScheme"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Texts.TextAutonumberScheme-enum. Representerar alla automatiska numreringsscheman"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textautonumberscheme/
---
## TextAutonumberScheme enumeration

Representerar alla automatiska numreringsscheman.

```csharp
public enum TextAutonumberScheme
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` |  |
| AlphaLcParenBoth | `1` | (a), (b), (c), … |
| AlphaLcParenR | `2` | a), b), c), … |
| AlphaLcPeriod | `3` | a., b., c., … |
| AlphaUcParenBoth | `4` | (A), (B), (C), … |
| AlphaUcParenR | `5` | A), B), C), … |
| AlphaUcPeriod | `6` | A., B., C., … |
| Arabic1Minus | `7` | Bidi Arabic 1 (AraAlpha) med ANSI minus‑symbol |
| Arabic2Minus | `8` | Bidi Arabic 2 (AraAbjad) med ANSI minus‑symbol |
| ArabicDbPeriod | `9` | Dubbla byte arabiska nummer med dubbelbyte‑punkt |
| ArabicDbPlain | `10` | Dubbla byte arabiska nummer |
| ArabicParenBoth | `11` | (1), (2), (3), … |
| ArabicParenR | `12` | 1), 2), 3), … |
| ArabicPeriod | `13` | 1., 2., 3., … |
| ArabicPlain | `14` | 1, 2, 3, … |
| CircleNumDbPlain | `15` | Dubbla byte cirkelnummmer (1-10 cirkel[0x2460-], 11-arabiska nummer) |
| CircleNumWdBlackPlain | `16` | Wingdings svarta cirkelnummmer |
| CircleNumWdWhitePlain | `17` | Wingdings vita cirkelnummmer (0-10 cirkel[0x0080-],11- arabiska nummer) |
| Ea1ChsPeriod | `18` | EA: Förenklad kinesiska med enkelbyte‑punkt |
| Ea1ChsPlain | `19` | EA: Förenklad kinesiska (TypA 1-99, TypC 100-) |
| Ea1ChtPeriod | `20` | EA: Traditionell kinesiska med enkelbyte‑punkt |
| Ea1ChtPlain | `21` | EA: Traditionell kinesiska (TypA 1-19, TypC 20-) |
| Ea1JpnChsDbPeriod | `22` | EA: Japanska med dubbelbyte‑punkt |
| Ea1JpnKorPeriod | `23` | EA: Japanska/Koreanska med enkelbyte‑punkt |
| Ea1JpnKorPlain | `24` | EA: Japanska/Koreanska (TypC 1-) |
| Hebrew2Minus | `25` | Bidi Hebrew 2 med ANSI minus‑symbol |
| HindiAlpha1Period | `26` | Hindi-alfabet punkt – konsonanter |
| HindiAlphaPeriod | `27` | Hindi-alfabet punkt – vokaler |
| HindiNumParenR | `28` | Hindi numeriska parenteser – höger |
| HindiNumPeriod | `29` | Hindi numerisk punkt |
| RomanLcParenBoth | `30` | (i), (ii), (iii), … |
| RomanLcParenR | `31` | i), ii), iii), … |
| RomanLcPeriod | `32` | i., ii., iii., … |
| RomanUcParenBoth | `33` | (I), (II), (III), … |
| RomanUcParenR | `34` | I), II), III), … |
| RomanUcPeriod | `35` | I., II., III., … |
| ThaiAlphaParenBoth | `36` | Thai-alfabet parenteser - båda |
| ThaiAlphaParenR | `37` | Thai-alfabet parenteser - höger |
| ThaiAlphaPeriod | `38` | Thai-alfabet punkt |
| ThaiNumParenBoth | `39` | Thai-numeriska parenteser - båda |
| ThaiNumParenR | `40` | Thai-numeriska parenteser - höger |
| ThaiNumPeriod | `41` | Thai-numerisk punkt |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextsClassTextAutonumberSchemeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textruta i kalkylbladet
            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            Aspose.Cells.Drawing.TextBox textbox = worksheet.TextBoxes[textboxIndex];
            
            // Ange text med olika autonummereringsscheman
            textbox.Text = "Autonumber Scheme Examples:\n\n";

            // Demonstrera olika TextAutonumberScheme‑värden
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.AlphaLcParenBoth, "Lowercase alpha with both parentheses");
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.AlphaUcPeriod, "Uppercase alpha with period");
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.ArabicParenR, "Arabic numbers with right parenthesis");
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.RomanLcPeriod, "Lowercase roman numerals with period");
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.CircleNumDbPlain, "Double-byte circle numbers");

            // Ange stycke med autonummereringsschema
            TextParagraphCollection paragraphs = textbox.TextBody.TextParagraphs;
            TextParagraph paragraph = paragraphs[paragraphs.Count - 1];
            paragraph.Bullet.Type = BulletType.AutoNumbered;
            ((AutoNumberedBulletValue)paragraph.Bullet.BulletValue).AutonumberScheme = TextAutonumberScheme.AlphaUcParenR;
            ((AutoNumberedBulletValue)paragraph.Bullet.BulletValue).StartAt = 1;

            // Spara arbetsboken
            workbook.Save("TextAutonumberSchemeDemo.xlsx");
        }

        private static string GetAutonumberExample(TextAutonumberScheme scheme, string description)
        {
            return $"{scheme.ToString()} ({description}):\n" +
                   "1. First item\n" +
                   "2. Second item\n" +
                   "3. Third item\n\n";
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


