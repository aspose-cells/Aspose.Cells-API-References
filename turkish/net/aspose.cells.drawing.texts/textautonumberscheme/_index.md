---
title: "Enum TextAutonumberScheme"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.Texts.TextAutonumberScheme enum'ı. Tüm otomatik numaralandırma şemasını temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing.texts/textautonumberscheme/
---
## TextAutonumberScheme enumeration

Tüm otomatik numaralandırma şemasını temsil eder.

```csharp
public enum TextAutonumberScheme
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` |  |
| AlphaLcParenBoth | `1` | (a), (b), (c), … |
| AlphaLcParenR | `2` | a), b), c), … |
| AlphaLcPeriod | `3` | a., b., c., … |
| AlphaUcParenBoth | `4` | (A), (B), (C), … |
| AlphaUcParenR | `5` | A), B), C), … |
| AlphaUcPeriod | `6` | A., B., C., … |
| Arabic1Minus | `7` | Bidi Arapça 1 (AraAlpha) ANSI eksi işareti ile |
| Arabic2Minus | `8` | Bidi Arapça 2 (AraAbjad) ANSI eksi işareti ile |
| ArabicDbPeriod | `9` | Çift baytlı Arapça sayılar çift baytlı nokta ile |
| ArabicDbPlain | `10` | Çift baytlı Arapça sayılar |
| ArabicParenBoth | `11` | (1), (2), (3), … |
| ArabicParenR | `12` | 1), 2), 3), … |
| ArabicPeriod | `13` | 1., 2., 3., … |
| ArabicPlain | `14` | 1, 2, 3, … |
| CircleNumDbPlain | `15` | Çift baytlı daire sayıları (1-10 daire[0x2460-], 11-arapça sayılar) |
| CircleNumWdBlackPlain | `16` | Wingdings siyah daire sayıları |
| CircleNumWdWhitePlain | `17` | Wingdings beyaz daire sayıları (0-10 daire[0x0080-],11- arapça sayılar) |
| Ea1ChsPeriod | `18` | EA: Basitleştirilmiş Çince tek baytlı nokta ile |
| Ea1ChsPlain | `19` | EA: Basitleştirilmiş Çince (TipA 1-99, TipC 100-) |
| Ea1ChtPeriod | `20` | EA: Geleneksel Çince w/ tek bayt nokta |
| Ea1ChtPlain | `21` | EA: Geleneksel Çince (TipA 1-19, TipC 20-) |
| Ea1JpnChsDbPeriod | `22` | EA: Japonca w/ çift bayt nokta |
| Ea1JpnKorPeriod | `23` | EA: Japonca/Korece w/ tek bayt nokta |
| Ea1JpnKorPlain | `24` | EA: Japonca/Korece (TipC 1-) |
| Hebrew2Minus | `25` | Bidi İbranice 2 ANSI eksi işareti ile |
| HindiAlpha1Period | `26` | Hint alfabesi nokta - ünsüzler |
| HindiAlphaPeriod | `27` | Hint alfabesi nokta - ünlüler |
| HindiNumParenR | `28` | Hint sayısal parantez - sağ |
| HindiNumPeriod | `29` | Hint sayısal nokta |
| RomanLcParenBoth | `30` | (i), (ii), (iii), … |
| RomanLcParenR | `31` | i), ii), iii), … |
| RomanLcPeriod | `32` | i., ii., iii., … |
| RomanUcParenBoth | `33` | (I), (II), (III), … |
| RomanUcParenR | `34` | I), II), III), … |
| RomanUcPeriod | `35` | I., II., III., … |
| ThaiAlphaParenBoth | `36` | Tay alfabesi parantez - her ikisi |
| ThaiAlphaParenR | `37` | Tay alfabesi parantez - sağ |
| ThaiAlphaPeriod | `38` | Tay alfabesi nokta |
| ThaiNumParenBoth | `39` | Tay sayısal parantez - her ikisi |
| ThaiNumParenR | `40` | Tay sayısal parantez - sağ |
| ThaiNumPeriod | `41` | Tay sayısal nokta |

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir metin kutusu ekle
            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            Aspose.Cells.Drawing.TextBox textbox = worksheet.TextBoxes[textboxIndex];
            
            // Metni farklı otomatik numaralandırma şemalarıyla ayarla
            textbox.Text = "Autonumber Scheme Examples:\n\n";

            // Çeşitli TextAutonumberScheme değerlerini göster
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.AlphaLcParenBoth, "Lowercase alpha with both parentheses");
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.AlphaUcPeriod, "Uppercase alpha with period");
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.ArabicParenR, "Arabic numbers with right parenthesis");
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.RomanLcPeriod, "Lowercase roman numerals with period");
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.CircleNumDbPlain, "Double-byte circle numbers");

            // Paragrafı otomatik numaralandırma şemasıyla ayarla
            TextParagraphCollection paragraphs = textbox.TextBody.TextParagraphs;
            TextParagraph paragraph = paragraphs[paragraphs.Count - 1];
            paragraph.Bullet.Type = BulletType.AutoNumbered;
            ((AutoNumberedBulletValue)paragraph.Bullet.BulletValue).AutonumberScheme = TextAutonumberScheme.AlphaUcParenR;
            ((AutoNumberedBulletValue)paragraph.Bullet.BulletValue).StartAt = 1;

            // Çalışma kitabını kaydedin
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

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


