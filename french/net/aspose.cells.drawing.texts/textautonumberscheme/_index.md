---
title: "Énumération TextAutonumberScheme"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.Drawing.Texts.TextAutonumberScheme. Représente tous les schémas de numérotation automatiques"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textautonumberscheme/
---
## TextAutonumberScheme enumeration

Représente tous les schémas de numérotation automatiques.

```csharp
public enum TextAutonumberScheme
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` |  |
| AlphaLcParenBoth | `1` | (a), (b), (c), … |
| AlphaLcParenR | `2` | a), b), c), … |
| AlphaLcPeriod | `3` | a., b., c., … |
| AlphaUcParenBoth | `4` | (A), (B), (C), … |
| AlphaUcParenR | `5` | A), B), C), … |
| AlphaUcPeriod | `6` | A., B., C., … |
| Arabic1Minus | `7` | Arabe Bidi 1 (AraAlpha) avec le symbole moins ANSI |
| Arabic2Minus | `8` | Arabe Bidi 2 (AraAbjad) avec le symbole moins ANSI |
| ArabicDbPeriod | `9` | Nombres arabes à double octet avec point double octet |
| ArabicDbPlain | `10` | Nombres arabes à double octet |
| ArabicParenBoth | `11` | (1), (2), (3), … |
| ArabicParenR | `12` | 1), 2), 3), … |
| ArabicPeriod | `13` | 1., 2., 3., … |
| ArabicPlain | `14` | 1, 2, 3, … |
| CircleNumDbPlain | `15` | Nombres cerclés à double octet (1-10 cercle[0x2460-], 11-nombres arabes) |
| CircleNumWdBlackPlain | `16` | Nombres à cercle noir Wingdings |
| CircleNumWdWhitePlain | `17` | Nombres à cercle blanc Wingdings (0-10 cercle[0x0080-], 11- nombres arabes) |
| Ea1ChsPeriod | `18` | EA : chinois simplifié avec point à simple octet |
| Ea1ChsPlain | `19` | EA: Chinois simplifié (TypeA 1-99, TypeC 100-) |
| Ea1ChtPeriod | `20` | EA: Chinois traditionnel avec point à octet unique |
| Ea1ChtPlain | `21` | EA: Chinois traditionnel (TypeA 1-19, TypeC 20-) |
| Ea1JpnChsDbPeriod | `22` | EA: Japonais avec point à double octet |
| Ea1JpnKorPeriod | `23` | EA: Japonais/Coréen avec point à octet unique |
| Ea1JpnKorPlain | `24` | EA: Japonais/Coréen (TypeC 1-) |
| Hebrew2Minus | `25` | Bidi Hébreu 2 avec symbole moins ANSI |
| HindiAlpha1Period | `26` | Alphabet hindi point - consonnes |
| HindiAlphaPeriod | `27` | Alphabet hindi point - voyelles |
| HindiNumParenR | `28` | Parenthèses numériques hindi - droite |
| HindiNumPeriod | `29` | Point numérique hindi |
| RomanLcParenBoth | `30` | (i), (ii), (iii), … |
| RomanLcParenR | `31` | i), ii), iii), … |
| RomanLcPeriod | `32` | i., ii., iii., … |
| RomanUcParenBoth | `33` | (I), (II), (III), … |
| RomanUcParenR | `34` | I), II), III), … |
| RomanUcPeriod | `35` | I., II., III., … |
| ThaiAlphaParenBoth | `36` | Alphabet thaï parenthèses - les deux |
| ThaiAlphaParenR | `37` | Alphabet thaï parenthèses - droite |
| ThaiAlphaPeriod | `38` | Alphabet thaï point |
| ThaiNumParenBoth | `39` | Parenthèses numériques thaï - les deux |
| ThaiNumParenR | `40` | Parenthèses numériques thaï - droite |
| ThaiNumPeriod | `41` | Point numérique thaï |

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une zone de texte à la feuille de calcul
            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            Aspose.Cells.Drawing.TextBox textbox = worksheet.TextBoxes[textboxIndex];
            
            // Définir le texte avec différents schémas d'auto-numérotation
            textbox.Text = "Autonumber Scheme Examples:\n\n";

            // Démontrer diverses valeurs de TextAutonumberScheme
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.AlphaLcParenBoth, "Lowercase alpha with both parentheses");
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.AlphaUcPeriod, "Uppercase alpha with period");
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.ArabicParenR, "Arabic numbers with right parenthesis");
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.RomanLcPeriod, "Lowercase roman numerals with period");
            textbox.Text += GetAutonumberExample(TextAutonumberScheme.CircleNumDbPlain, "Double-byte circle numbers");

            // Définir le paragraphe avec le schéma de numérotation automatique
            TextParagraphCollection paragraphs = textbox.TextBody.TextParagraphs;
            TextParagraph paragraph = paragraphs[paragraphs.Count - 1];
            paragraph.Bullet.Type = BulletType.AutoNumbered;
            ((AutoNumberedBulletValue)paragraph.Bullet.BulletValue).AutonumberScheme = TextAutonumberScheme.AlphaUcParenR;
            ((AutoNumberedBulletValue)paragraph.Bullet.BulletValue).StartAt = 1;

            // Enregistrez le classeur
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

### Voir aussi

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


