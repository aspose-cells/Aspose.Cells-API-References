##Enum TextAutonumberScheme
Aspose.Cells.Drawing.Texts.TextAutonumberScheme enum. Represents all automatic number scheme
## TextAutonumberScheme enumeration
Represents all automatic number scheme.
```csharp
public enum TextAutonumberScheme
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` |  |
| AlphaLcParenBoth | `1` | (a), (b), (c), … |
| AlphaLcParenR | `2` | a), b), c), … |
| AlphaLcPeriod | `3` | a., b., c., … |
| AlphaUcParenBoth | `4` | (A), (B), (C), … |
| AlphaUcParenR | `5` | A), B), C), … |
| AlphaUcPeriod | `6` | A., B., C., … |
| Arabic1Minus | `7` | Bidi Arabic 1 (AraAlpha) with ANSI minus symbol |
| Arabic2Minus | `8` | Bidi Arabic 2 (AraAbjad) with ANSI minus symbol |
| ArabicDbPeriod | `9` | Dbl-byte Arabic numbers w/ double-byte period |
| ArabicDbPlain | `10` | Dbl-byte Arabic numbers |
| ArabicParenBoth | `11` | (1), (2), (3), … |
| ArabicParenR | `12` | 1), 2), 3), … |
| ArabicPeriod | `13` | 1., 2., 3., … |
| ArabicPlain | `14` | 1, 2, 3, … |
| CircleNumDbPlain | `15` | Dbl-byte circle numbers (1-10 circle[0x2460-], 11-arabic numbers) |
| CircleNumWdBlackPlain | `16` | Wingdings black circle numbers |
| CircleNumWdWhitePlain | `17` | Wingdings white circle numbers (0-10 circle[0x0080-],11- arabic numbers) |
| Ea1ChsPeriod | `18` | EA: Simplified Chinese w/ single-byte period |
| Ea1ChsPlain | `19` | EA: Simplified Chinese (TypeA 1-99, TypeC 100-) |
| Ea1ChtPeriod | `20` | EA: Traditional Chinese w/ single-byte period |
| Ea1ChtPlain | `21` | EA: Traditional Chinese (TypeA 1-19, TypeC 20-) |
| Ea1JpnChsDbPeriod | `22` | EA: Japanese w/ double-byte period |
| Ea1JpnKorPeriod | `23` | EA: Japanese/Korean w/ single-byte period |
| Ea1JpnKorPlain | `24` | EA: Japanese/Korean (TypeC 1-) |
| Hebrew2Minus | `25` | Bidi Hebrew 2 with ANSI minus symbol |
| HindiAlpha1Period | `26` | Hindi alphabet period - consonants |
| HindiAlphaPeriod | `27` | Hindi alphabet period - vowels |
| HindiNumParenR | `28` | Hindi numerical parentheses - right |
| HindiNumPeriod | `29` | Hindi numerical period |
| RomanLcParenBoth | `30` | (i), (ii), (iii), … |
| RomanLcParenR | `31` | i), ii), iii), … |
| RomanLcPeriod | `32` | i., ii., iii., … |
| RomanUcParenBoth | `33` | (I), (II), (III), … |
| RomanUcParenR | `34` | I), II), III), … |
| RomanUcPeriod | `35` | I., II., III., … |
| ThaiAlphaParenBoth | `36` | Thai alphabet parentheses - both |
| ThaiAlphaParenR | `37` | Thai alphabet parentheses - right |
| ThaiAlphaPeriod | `38` | Thai alphabet period |
| ThaiNumParenBoth | `39` | Thai numerical parentheses - both |
| ThaiNumParenR | `40` | Thai numerical parentheses - right |
| ThaiNumPeriod | `41` | Thai numerical period |
### Examples
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
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box to the worksheet
int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
Aspose.Cells.Drawing.TextBox textbox = worksheet.TextBoxes[textboxIndex];
// Set text with different autonumber schemes
textbox.Text = "Autonumber Scheme Examples:\n\n";
// Demonstrate various TextAutonumberScheme values
textbox.Text += GetAutonumberExample(TextAutonumberScheme.AlphaLcParenBoth, "Lowercase alpha with both parentheses");
textbox.Text += GetAutonumberExample(TextAutonumberScheme.AlphaUcPeriod, "Uppercase alpha with period");
textbox.Text += GetAutonumberExample(TextAutonumberScheme.ArabicParenR, "Arabic numbers with right parenthesis");
textbox.Text += GetAutonumberExample(TextAutonumberScheme.RomanLcPeriod, "Lowercase roman numerals with period");
textbox.Text += GetAutonumberExample(TextAutonumberScheme.CircleNumDbPlain, "Double-byte circle numbers");
// Set paragraph with autonumber scheme
TextParagraphCollection paragraphs = textbox.TextBody.TextParagraphs;
TextParagraph paragraph = paragraphs[paragraphs.Count - 1];
paragraph.Bullet.Type = BulletType.AutoNumbered;
((AutoNumberedBulletValue)paragraph.Bullet.BulletValue).AutonumberScheme = TextAutonumberScheme.AlphaUcParenR;
((AutoNumberedBulletValue)paragraph.Bullet.BulletValue).StartAt = 1;
// Save the workbook
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
### See Also
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)
