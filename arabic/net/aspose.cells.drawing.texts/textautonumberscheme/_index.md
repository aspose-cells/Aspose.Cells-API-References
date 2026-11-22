---
title: "التعداد TextAutonumberScheme"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Drawing.Texts.TextAutonumberScheme. يمثل جميع مخططات الأرقام التلقائية"
type: docs
url: /ar/net/aspose.cells.drawing.texts/textautonumberscheme/
---
## TextAutonumberScheme enumeration

يمثل جميع مخططات الأرقام التلقائية.

```csharp
public enum TextAutonumberScheme
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` |  |
| AlphaLcParenBoth | `1` | (a), (b), (c), … |
| AlphaLcParenR | `2` | a), b), c), … |
| AlphaLcPeriod | `3` | a., b., c., … |
| AlphaUcParenBoth | `4` | (A), (B), (C), … |
| AlphaUcParenR | `5` | A), B), C), … |
| AlphaUcPeriod | `6` | A., B., C., … |
| Arabic1Minus | `7` | العربية ثنائية الاتجاه 1 (AraAlpha) مع رمز الطرح ANSI |
| Arabic2Minus | `8` | العربية ثنائية الاتجاه 2 (AraAbjad) مع رمز الطرح ANSI |
| ArabicDbPeriod | `9` | أرقام عربية ذات بايت مزدوج مع نقطة مزدوجة البايت |
| ArabicDbPlain | `10` | أرقام عربية ذات بايت مزدوج |
| ArabicParenBoth | `11` | (1), (2), (3), … |
| ArabicParenR | `12` | 1), 2), 3), … |
| ArabicPeriod | `13` | 1., 2., 3., … |
| ArabicPlain | `14` | 1, 2, 3, … |
| CircleNumDbPlain | `15` | أرقام دائرية ذات بايت مزدوج (1-10 دائرة[0x2460-]، 11-أرقام عربية) |
| CircleNumWdBlackPlain | `16` | أرقام دائرة سوداء Wingdings |
| CircleNumWdWhitePlain | `17` | أرقام دائرة بيضاء Wingdings (0-10 دائرة[0x0080-]، 11- أرقام عربية) |
| Ea1ChsPeriod | `18` | EA: صينية مبسطة مع نقطة بايت واحد |
| Ea1ChsPlain | `19` | EA: الصينية المبسطة (TypeA 1-99, TypeC 100-) |
| Ea1ChtPeriod | `20` | EA: الصينية التقليدية مع نقطة أحادية البايت |
| Ea1ChtPlain | `21` | EA: الصينية التقليدية (TypeA 1-19, TypeC 20-) |
| Ea1JpnChsDbPeriod | `22` | EA: اليابانية مع نقطة مزدوجة البايت |
| Ea1JpnKorPeriod | `23` | EA: اليابانية/الكورية مع نقطة أحادية البايت |
| Ea1JpnKorPlain | `24` | EA: اليابانية/الكورية (TypeC 1-) |
| Hebrew2Minus | `25` | Bidi العبرية 2 مع رمز الطرح ANSI |
| HindiAlpha1Period | `26` | الأبجدية الهندية نقطة - الحروف الساكنة |
| HindiAlphaPeriod | `27` | الأبجدية الهندية نقطة - الحروف المتحركة |
| HindiNumParenR | `28` | الأرقام الهندية أقواس - يمين |
| HindiNumPeriod | `29` | الأرقام الهندية نقطة |
| RomanLcParenBoth | `30` | (i), (ii), (iii), … |
| RomanLcParenR | `31` | i), ii), iii), … |
| RomanLcPeriod | `32` | i., ii., iii., … |
| RomanUcParenBoth | `33` | (I), (II), (III), … |
| RomanUcParenR | `34` | I), II), III), … |
| RomanUcPeriod | `35` | I., II., III., … |
| ThaiAlphaParenBoth | `36` | الأبجدية التايلاندية أقواس - كلا |
| ThaiAlphaParenR | `37` | الأبجدية التايلاندية أقواس - يمين |
| ThaiAlphaPeriod | `38` | الأبجدية التايلاندية نقطة |
| ThaiNumParenBoth | `39` | الأرقام التايلاندية أقواس - كلا |
| ThaiNumParenR | `40` | الأرقام التايلاندية أقواس - يمين |
| ThaiNumPeriod | `41` | الأرقام التايلاندية نقطة |

### أمثلة

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
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة مربع نص إلى ورقة العمل
            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            Aspose.Cells.Drawing.TextBox textbox = worksheet.TextBoxes[textboxIndex];
            
            // ضبط النص مع مخططات الترقيم التلقائي المختلفة
            textbox.Text = "Autonumber Scheme Examples:\n\n";

            // عرض قيم TextAutonumberScheme المختلفة
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.AlphaLcParenBoth, "Lowercase alpha with both parentheses");
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.AlphaUcPeriod, "Uppercase alpha with period");
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.ArabicParenR, "Arabic numbers with right parenthesis");
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.RomanLcPeriod, "Lowercase roman numerals with period");
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.CircleNumDbPlain, "Double-byte circle numbers");

            // تعيين فقرة باستخدام مخطط الترقيم التلقائي
            TextParagraphCollection paragraphs = textbox.TextBody.TextParagraphs;
            TextParagraph paragraph = paragraphs[paragraphs.Count - 1];
            paragraph.Bullet.Type = BulletType.AutoNumbered;
            ((AutoNumberedBulletValue)paragraph.Bullet.BulletValue).AutonumberScheme = TextAutonumberScheme.AlphaUcParenR;
            ((AutoNumberedBulletValue)paragraph.Bullet.BulletValue).StartAt = 1;

            // احفظ المصنف
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

### انظر أيضًا

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


