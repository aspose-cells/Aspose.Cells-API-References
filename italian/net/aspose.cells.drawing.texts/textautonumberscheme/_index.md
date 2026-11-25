---
title: "Enum TextAutonumberScheme"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Drawing.Texts.TextAutonumberScheme. Rappresenta tutti gli schemi di numerazione automatica"
type: docs
url: /it/net/aspose.cells.drawing.texts/textautonumberscheme/
---
## TextAutonumberScheme enumeration

Rappresenta tutti gli schemi di numerazione automatici.

```csharp
public enum TextAutonumberScheme
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` |  |
| AlphaLcParenBoth | `1` | (a), (b), (c), … |
| AlphaLcParenR | `2` | a), b), c), … |
| AlphaLcPeriod | `3` | a., b., c., … |
| AlphaUcParenBoth | `4` | (A), (B), (C), … |
| AlphaUcParenR | `5` | A), B), C), … |
| AlphaUcPeriod | `6` | A., B., C., … |
| Arabic1Minus | `7` | Arabo Bidi 1 (AraAlpha) con simbolo meno ANSI |
| Arabic2Minus | `8` | Arabo Bidi 2 (AraAbjad) con simbolo meno ANSI |
| ArabicDbPeriod | `9` | Numeri arabi a doppio byte con punto a doppio byte |
| ArabicDbPlain | `10` | Numeri arabi a doppio byte |
| ArabicParenBoth | `11` | (1), (2), (3), … |
| ArabicParenR | `12` | 1), 2), 3), … |
| ArabicPeriod | `13` | 1., 2., 3., … |
| ArabicPlain | `14` | 1, 2, 3, … |
| CircleNumDbPlain | `15` | Numeri cerchi a doppio byte (1-10 cerchio[0x2460-], 11-numeri arabi) |
| CircleNumWdBlackPlain | `16` | Numeri cerchio neri Wingdings |
| CircleNumWdWhitePlain | `17` | Numeri cerchio bianchi Wingdings (0-10 cerchio[0x0080-], 11- numeri arabi) |
| Ea1ChsPeriod | `18` | EA: Cinese semplificato con punto a singolo byte |
| Ea1ChsPlain | `19` | EA: Cinese semplificato (TypeA 1-99, TypeC 100-) |
| Ea1ChtPeriod | `20` | EA: Cinese tradizionale con punto a byte singolo |
| Ea1ChtPlain | `21` | EA: Cinese tradizionale (TypeA 1-19, TypeC 20-) |
| Ea1JpnChsDbPeriod | `22` | EA: Giapponese con punto a doppio byte |
| Ea1JpnKorPeriod | `23` | EA: Giapponese/Koreano con punto a byte singolo |
| Ea1JpnKorPlain | `24` | EA: Giapponese/Koreano (TypeC 1-) |
| Hebrew2Minus | `25` | Ebraico Bidi 2 con simbolo meno ANSI |
| HindiAlpha1Period | `26` | Alfabeto Hindi punto - consonanti |
| HindiAlphaPeriod | `27` | Alfabeto Hindi punto - vocali |
| HindiNumParenR | `28` | Parentesi numeriche Hindi - destra |
| HindiNumPeriod | `29` | Punto numerico Hindi |
| RomanLcParenBoth | `30` | (i), (ii), (iii), … |
| RomanLcParenR | `31` | i), ii), iii), … |
| RomanLcPeriod | `32` | i., ii., iii., … |
| RomanUcParenBoth | `33` | (I), (II), (III), … |
| RomanUcParenR | `34` | I), II), III), … |
| RomanUcPeriod | `35` | I., II., III., … |
| ThaiAlphaParenBoth | `36` | Parentesi alfabeto Thai - entrambe |
| ThaiAlphaParenR | `37` | Parentesi alfabeto Thai - destra |
| ThaiAlphaPeriod | `38` | Punto alfabeto Thai |
| ThaiNumParenBoth | `39` | Parentesi numeriche Thai - entrambe |
| ThaiNumParenR | `40` | Parentesi numeriche Thai - destra |
| ThaiNumPeriod | `41` | Punto numerico Thai |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una casella di testo al foglio di lavoro
            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            Aspose.Cells.Drawing.TextBox textbox = worksheet.TextBoxes[textboxIndex];
            
            // Imposta il testo con diversi schemi di numerazione automatica
            textbox.Text = "Autonumber Scheme Examples:\n\n";

            // Dimostra vari valori di TextAutonumberScheme
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.AlphaLcParenBoth, "Lowercase alpha with both parentheses");
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.AlphaUcPeriod, "Uppercase alpha with period");
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.ArabicParenR, "Arabic numbers with right parenthesis");
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.RomanLcPeriod, "Lowercase roman numerals with period");
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.CircleNumDbPlain, "Double-byte circle numbers");

            // Imposta il paragrafo con schema di numerazione automatica
            TextParagraphCollection paragraphs = textbox.TextBody.TextParagraphs;
            TextParagraph paragraph = paragraphs[paragraphs.Count - 1];
            paragraph.Bullet.Type = BulletType.AutoNumbered;
            ((AutoNumberedBulletValue)paragraph.Bullet.BulletValue).AutonumberScheme = TextAutonumberScheme.AlphaUcParenR;
            ((AutoNumberedBulletValue)paragraph.Bullet.BulletValue).StartAt = 1;

            // Salva la cartella di lavoro
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

### Vedi anche

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


