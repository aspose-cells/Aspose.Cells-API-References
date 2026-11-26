---
title: "Enum TextAutonumberScheme"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.Drawing.Texts.TextAutonumberScheme. Representa todos los esquemas de numeración automática"
type: docs
url: /es/net/aspose.cells.drawing.texts/textautonumberscheme/
---
## TextAutonumberScheme enumeration

Representa todos los esquemas de numeración automática.

```csharp
public enum TextAutonumberScheme
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` |  |
| AlphaLcParenBoth | `1` | (a), (b), (c), … |
| AlphaLcParenR | `2` | a), b), c), … |
| AlphaLcPeriod | `3` | a., b., c., … |
| AlphaUcParenBoth | `4` | (A), (B), (C), … |
| AlphaUcParenR | `5` | A), B), C), … |
| AlphaUcPeriod | `6` | A., B., C., … |
| Arabic1Minus | `7` | Árabe bidi 1 (AraAlpha) con símbolo menos ANSI |
| Arabic2Minus | `8` | Árabe bidi 2 (AraAbjad) con símbolo menos ANSI |
| ArabicDbPeriod | `9` | Números árabes de doble byte con punto de doble byte |
| ArabicDbPlain | `10` | Números árabes de doble byte |
| ArabicParenBoth | `11` | (1), (2), (3), … |
| ArabicParenR | `12` | 1), 2), 3), … |
| ArabicPeriod | `13` | 1., 2., 3., … |
| ArabicPlain | `14` | 1, 2, 3, … |
| CircleNumDbPlain | `15` | Números circulares de doble byte (1-10 círculo[0x2460-], 11-números árabes) |
| CircleNumWdBlackPlain | `16` | Números de círculo negro Wingdings |
| CircleNumWdWhitePlain | `17` | Números de círculo blanco Wingdings (0-10 círculo[0x0080-],11- números árabes) |
| Ea1ChsPeriod | `18` | EA: Chino simplificado con punto de un solo byte |
| Ea1ChsPlain | `19` | EA: Chino simplificado (TypeA 1-99, TypeC 100-) |
| Ea1ChtPeriod | `20` | EA: Chino tradicional con punto de un solo byte |
| Ea1ChtPlain | `21` | EA: Chino tradicional (TypeA 1-19, TypeC 20-) |
| Ea1JpnChsDbPeriod | `22` | EA: Japonés con punto de doble byte |
| Ea1JpnKorPeriod | `23` | EA: Japonés/Coreano con punto de un solo byte |
| Ea1JpnKorPlain | `24` | EA: Japonés/Coreano (TypeC 1-) |
| Hebrew2Minus | `25` | Bidi hebreo 2 con símbolo menos ANSI |
| HindiAlpha1Period | `26` | Alfabeto hindi con punto - consonantes |
| HindiAlphaPeriod | `27` | Alfabeto hindi con punto - vocales |
| HindiNumParenR | `28` | Paréntesis numéricos hindi - derecha |
| HindiNumPeriod | `29` | Punto numérico hindi |
| RomanLcParenBoth | `30` | (i), (ii), (iii), … |
| RomanLcParenR | `31` | i), ii), iii), … |
| RomanLcPeriod | `32` | i., ii., iii., … |
| RomanUcParenBoth | `33` | (I), (II), (III), … |
| RomanUcParenR | `34` | I), II), III), … |
| RomanUcPeriod | `35` | I., II., III., … |
| ThaiAlphaParenBoth | `36` | Paréntesis alfabeto tailandés - ambos |
| ThaiAlphaParenR | `37` | Paréntesis alfabeto tailandés - derecha |
| ThaiAlphaPeriod | `38` | Punto alfabeto tailandés |
| ThaiNumParenBoth | `39` | Paréntesis numéricos tailandeses - ambos |
| ThaiNumParenR | `40` | Paréntesis numéricos tailandeses - derecha |
| ThaiNumPeriod | `41` | Punto numérico tailandés |

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un cuadro de texto a la hoja de cálculo
            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            Aspose.Cells.Drawing.TextBox textbox = worksheet.TextBoxes[textboxIndex];
            
            // Establecer texto con diferentes esquemas de autonumeración
            textbox.Text = "Autonumber Scheme Examples:\n\n";

            // Demostrar varios valores de TextAutonumberScheme
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.AlphaLcParenBoth, "Lowercase alpha with both parentheses");
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.AlphaUcPeriod, "Uppercase alpha with period");
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.ArabicParenR, "Arabic numbers with right parenthesis");
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.RomanLcPeriod, "Lowercase roman numerals with period");
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.CircleNumDbPlain, "Double-byte circle numbers");

            // Establecer párrafo con esquema de numeración automática
            TextParagraphCollection paragraphs = textbox.TextBody.TextParagraphs;
            TextParagraph paragraph = paragraphs[paragraphs.Count - 1];
            paragraph.Bullet.Type = BulletType.AutoNumbered;
            ((AutoNumberedBulletValue)paragraph.Bullet.BulletValue).AutonumberScheme = TextAutonumberScheme.AlphaUcParenR;
            ((AutoNumberedBulletValue)paragraph.Bullet.BulletValue).StartAt = 1;

            // Guarda el libro de trabajo
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

### Ver también

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


