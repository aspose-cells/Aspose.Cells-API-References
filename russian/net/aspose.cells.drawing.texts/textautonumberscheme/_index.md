---
title: "Перечисление TextAutonumberScheme"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.Texts.TextAutonumberScheme. Представляет все схемы автоматической нумерации"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textautonumberscheme/
---
## TextAutonumberScheme enumeration

Представляет все схемы автоматической нумерации.

```csharp
public enum TextAutonumberScheme
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` |  |
| AlphaLcParenBoth | `1` | (a), (b), (c), … |
| AlphaLcParenR | `2` | a), b), c), … |
| AlphaLcPeriod | `3` | a., b., c., … |
| AlphaUcParenBoth | `4` | (A), (B), (C), … |
| AlphaUcParenR | `5` | A), B), C), … |
| AlphaUcPeriod | `6` | A., B., C., … |
| Arabic1Minus | `7` | Bidi Arabic 1 (AraAlpha) с символом минуса ANSI |
| Arabic2Minus | `8` | Bidi Arabic 2 (AraAbjad) с символом минуса ANSI |
| ArabicDbPeriod | `9` | Dbl-byte арабские цифры с двойным байтовым знаком точки |
| ArabicDbPlain | `10` | Dbl-byte арабские цифры |
| ArabicParenBoth | `11` | (1), (2), (3), … |
| ArabicParenR | `12` | 1), 2), 3), … |
| ArabicPeriod | `13` | 1., 2., 3., … |
| ArabicPlain | `14` | 1, 2, 3, … |
| CircleNumDbPlain | `15` | Dbl-byte круглые числа (1-10 круг[0x2460-], 11-арабские цифры) |
| CircleNumWdBlackPlain | `16` | Wingdings черные круглые числа |
| CircleNumWdWhitePlain | `17` | Wingdings белые круглые числа (0-10 круг[0x0080-], 11- арабские цифры) |
| Ea1ChsPeriod | `18` | EA: Упрощенный китайский с однобайтовым знаком точки |
| Ea1ChsPlain | `19` | EA: упрощённый китайский (TypeA 1-99, TypeC 100-) |
| Ea1ChtPeriod | `20` | EA: традиционный китайский с однобайтовой точкой |
| Ea1ChtPlain | `21` | EA: традиционный китайский (TypeA 1-19, TypeC 20-) |
| Ea1JpnChsDbPeriod | `22` | EA: японский с двойной байтовой точкой |
| Ea1JpnKorPeriod | `23` | EA: японский/корейский с однобайтовой точкой |
| Ea1JpnKorPlain | `24` | EA: японский/корейский (TypeC 1-) |
| Hebrew2Minus | `25` | Bidi Hebrew 2 с ANSI-минусом |
| HindiAlpha1Period | `26` | Хинди алфавит точка - согласные |
| HindiAlphaPeriod | `27` | Хинди алфавит точка - гласные |
| HindiNumParenR | `28` | Хинди числовые скобки - справа |
| HindiNumPeriod | `29` | Хинди числовая точка |
| RomanLcParenBoth | `30` | (i), (ii), (iii), … |
| RomanLcParenR | `31` | i), ii), iii), … |
| RomanLcPeriod | `32` | i., ii., iii., … |
| RomanUcParenBoth | `33` | (I), (II), (III), … |
| RomanUcParenR | `34` | I), II), III), … |
| RomanUcPeriod | `35` | I., II., III., … |
| ThaiAlphaParenBoth | `36` | Тайский алфавит скобки - оба |
| ThaiAlphaParenR | `37` | Тайский алфавит скобки - справа |
| ThaiAlphaPeriod | `38` | Тайский алфавит точка |
| ThaiNumParenBoth | `39` | Тайские числовые скобки - оба |
| ThaiNumParenR | `40` | Тайские числовые скобки - справа |
| ThaiNumPeriod | `41` | Тайская числовая точка |

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить текстовое поле на лист
            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            Aspose.Cells.Drawing.TextBox textbox = worksheet.TextBoxes[textboxIndex];
            
            // Установить текст с различными схемами автонумерации
            textbox.Text = "Autonumber Scheme Examples:\n\n";

            // Продемонстрировать различные значения **TextAutonumberScheme**
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.AlphaLcParenBoth, "Lowercase alpha with both parentheses");
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.AlphaUcPeriod, "Uppercase alpha with period");
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.ArabicParenR, "Arabic numbers with right parenthesis");
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.RomanLcPeriod, "Lowercase roman numerals with period");
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.CircleNumDbPlain, "Double-byte circle numbers");

            // Установить абзац с схемой автонумерации
            TextParagraphCollection paragraphs = textbox.TextBody.TextParagraphs;
            TextParagraph paragraph = paragraphs[paragraphs.Count - 1];
            paragraph.Bullet.Type = BulletType.AutoNumbered;
            ((AutoNumberedBulletValue)paragraph.Bullet.BulletValue).AutonumberScheme = TextAutonumberScheme.AlphaUcParenR;
            ((AutoNumberedBulletValue)paragraph.Bullet.BulletValue).StartAt = 1;

            // Сохраните книгу
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

### См. также

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


