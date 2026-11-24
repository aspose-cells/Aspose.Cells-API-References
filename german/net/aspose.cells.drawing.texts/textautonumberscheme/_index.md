---
title: "Enum TextAutonumberScheme"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.Texts.TextAutonumberScheme enum. Stellt alle automatischen Nummerierungsschemata dar"
type: docs
url: /de/net/aspose.cells.drawing.texts/textautonumberscheme/
---
## TextAutonumberScheme enumeration

Stellt alle automatischen Nummerierungsschemata dar.

```csharp
public enum TextAutonumberScheme
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` |  |
| AlphaLcParenBoth | `1` | (a), (b), (c), … |
| AlphaLcParenR | `2` | a), b), c), … |
| AlphaLcPeriod | `3` | a., b., c., … |
| AlphaUcParenBoth | `4` | (A), (B), (C), … |
| AlphaUcParenR | `5` | A), B), C), … |
| AlphaUcPeriod | `6` | A., B., C., … |
| Arabic1Minus | `7` | Bidi Arabic 1 (AraAlpha) mit ANSI-Minus-Symbol |
| Arabic2Minus | `8` | Bidi Arabic 2 (AraAbjad) mit ANSI‑Minuszeichen |
| ArabicDbPeriod | `9` | Doppelbyte Arabische Zahlen mit Doppelbyte‑Punkt |
| ArabicDbPlain | `10` | Doppelbyte Arabische Zahlen |
| ArabicParenBoth | `11` | (1), (2), (3), … |
| ArabicParenR | `12` | 1), 2), 3), … |
| ArabicPeriod | `13` | 1., 2., 3., … |
| ArabicPlain | `14` | 1, 2, 3, … |
| CircleNumDbPlain | `15` | Doppelbyte Kreiszahlen (1‑10 Kreis[0x2460-], 11‑arabische Zahlen) |
| CircleNumWdBlackPlain | `16` | Wingdings schwarze Kreiszahlen |
| CircleNumWdWhitePlain | `17` | Wingdings weiße Kreiszahlen (0‑10 Kreis[0x0080-],11‑ arabische Zahlen) |
| Ea1ChsPeriod | `18` | EA: Vereinfachtes Chinesisch mit Einzelbyte‑Punkt |
| Ea1ChsPlain | `19` | EA: Vereinfachtes Chinesisch (TypeA 1‑99, TypeC 100‑) |
| Ea1ChtPeriod | `20` | EA: Traditionelles Chinesisch mit Einzelbyte‑Punkt |
| Ea1ChtPlain | `21` | EA: Traditionelles Chinesisch (TypeA 1‑19, TypeC 20‑) |
| Ea1JpnChsDbPeriod | `22` | EA: Japanisch mit Doppelbyte‑Punkt |
| Ea1JpnKorPeriod | `23` | EA: Japanisch/Koreanisch mit Einzelbyte‑Punkt |
| Ea1JpnKorPlain | `24` | EA: Japanisch/Koreanisch (TypeC 1‑) |
| Hebrew2Minus | `25` | Bidi Hebräisch 2 mit ANSI‑Minuszeichen |
| HindiAlpha1Period | `26` | Hindi‑Alphabet Punkt – Konsonanten |
| HindiAlphaPeriod | `27` | Hindi‑Alphabet Punkt – Vokale |
| HindiNumParenR | `28` | Hindi‑Numerische Klammern – rechts |
| HindiNumPeriod | `29` | Hindi‑Numerischer Punkt |
| RomanLcParenBoth | `30` | (i), (ii), (iii), … |
| RomanLcParenR | `31` | i), ii), iii), … |
| RomanLcPeriod | `32` | i., ii., iii., … |
| RomanUcParenBoth | `33` | (I), (II), (III), … |
| RomanUcParenR | `34` | I), II), III), … |
| RomanUcPeriod | `35` | I., II., III., … |
| ThaiAlphaParenBoth | `36` | Thai-Alphabet-Klammern - beide |
| ThaiAlphaParenR | `37` | Thai-Alphabet-Klammern - rechts |
| ThaiAlphaPeriod | `38` | Thai-Alphabet-Punkt |
| ThaiNumParenBoth | `39` | Thai-Ziffern-Klammern - beide |
| ThaiNumParenR | `40` | Thai-Ziffern-Klammern - rechts |
| ThaiNumPeriod | `41` | Thai-Ziffern-Punkt |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Textfeld zum Arbeitsblatt hinzu
            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            Aspose.Cells.Drawing.TextBox textbox = worksheet.TextBoxes[textboxIndex];
            
            // Text mit verschiedenen automatischen Nummerierungsschemata festlegen
            textbox.Text = "Autonumber Scheme Examples:\n\n";

            // Verschiedene Werte von TextAutonumberScheme demonstrieren
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.AlphaLcParenBoth, "Lowercase alpha with both parentheses");
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.AlphaUcPeriod, "Uppercase alpha with period");
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.ArabicParenR, "Arabic numbers with right parenthesis");
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.RomanLcPeriod, "Lowercase roman numerals with period");
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.CircleNumDbPlain, "Double-byte circle numbers");

            // Absatz mit automatischem Nummerierungsschema festlegen
            TextParagraphCollection paragraphs = textbox.TextBody.TextParagraphs;
            TextParagraph paragraph = paragraphs[paragraphs.Count - 1];
            paragraph.Bullet.Type = BulletType.AutoNumbered;
            ((AutoNumberedBulletValue)paragraph.Bullet.BulletValue).AutonumberScheme = TextAutonumberScheme.AlphaUcParenR;
            ((AutoNumberedBulletValue)paragraph.Bullet.BulletValue).StartAt = 1;

            // Speichere die Arbeitsmappe
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

### Siehe auch

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


