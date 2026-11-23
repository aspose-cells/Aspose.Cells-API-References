---
title: "Classe TextParagraph"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.Texts.TextParagraph classe. Représente le paramètre du paragraphe de texte"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textparagraph/
---
## TextParagraph class

Représente le paramètre de paragraphe texte.

```csharp
public class TextParagraph : FontSetting
```

## Propriétés

| Nom | Description |
| --- | --- |
| [AlignmentType](../../aspose.cells.drawing.texts/textparagraph/alignmenttype/) { get; set; } | Obtient et définit le type d'alignement horizontal du texte du paragraphe. |
| [Bullet](../../aspose.cells.drawing.texts/textparagraph/bullet/) { get; } | Obtient la puce. |
| [Children](../../aspose.cells.drawing.texts/textparagraph/children/) { get; } | Obtient toutes les séquences de texte dans ce paragraphe. Si ce paragraphe est vide, renvoie le paragraphe lui‑même. |
| [DefaultTabSize](../../aspose.cells.drawing.texts/textparagraph/defaulttabsize/) { get; set; } | Obtient et définit la taille par défaut d'un caractère de tabulation dans ce paragraphe. |
| [FirstLineIndent](../../aspose.cells.drawing.texts/textparagraph/firstlineindent/) { get; set; } | Spécifie la taille du retrait qui sera appliquée à la première ligne de texte du paragraphe. |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Renvoie la police de cet objet. (Hérité de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [FontAlignType](../../aspose.cells.drawing.texts/textparagraph/fontaligntype/) { get; set; } | Détermine où, verticalement, sur une ligne de texte, les mots réels sont positionnés. Cela concerne le placement vertical des caractères par rapport aux lignes de base. |
| [IsEastAsianLineBreak](../../aspose.cells.drawing.texts/textparagraph/iseastasianlinebreak/) { get; set; } | Spécifie si un mot d'Asie de l'Est peut être coupé en deux et renvoyé à la ligne suivante sans ajouter de trait d'union. |
| [IsHangingPunctuation](../../aspose.cells.drawing.texts/textparagraph/ishangingpunctuation/) { get; set; } | Spécifie si la ponctuation doit être forcée à se placer sur une ligne de texte ou mise sur une ligne de texte différente. |
| [IsLatinLineBreak](../../aspose.cells.drawing.texts/textparagraph/islatinlinebreak/) { get; set; } | Spécifie si un mot latin peut être coupé en deux et renvoyé à la ligne suivante sans ajouter de trait d'union. |
| [LeftMargin](../../aspose.cells.drawing.texts/textparagraph/leftmargin/) { get; set; } | Spécifie la marge gauche du paragraphe. |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Obtient la longueur des caractères. (Hérité de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [LineSpace](../../aspose.cells.drawing.texts/textparagraph/linespace/) { get; set; } | Obtient et définit la quantité d'espace blanc vertical qui sera utilisé dans un paragraphe. |
| [LineSpaceSizeType](../../aspose.cells.drawing.texts/textparagraph/linespacesizetype/) { get; set; } | Obtient et définit la quantité d'espace blanc vertical qui sera utilisé dans un paragraphe. |
| [RightMargin](../../aspose.cells.drawing.texts/textparagraph/rightmargin/) { get; set; } | Spécifie la marge droite du paragraphe. |
| [SpaceAfter](../../aspose.cells.drawing.texts/textparagraph/spaceafter/) { get; set; } | Obtient et définit la quantité d'espace blanc vertical qui sera présent après un paragraphe. |
| [SpaceAfterSizeType](../../aspose.cells.drawing.texts/textparagraph/spaceaftersizetype/) { get; set; } | Obtient et définit la quantité d'espace blanc vertical qui sera présent après un paragraphe. |
| [SpaceBefore](../../aspose.cells.drawing.texts/textparagraph/spacebefore/) { get; set; } | Obtient et définit la quantité d'espace blanc vertical qui sera présent avant un paragraphe. |
| [SpaceBeforeSizeType](../../aspose.cells.drawing.texts/textparagraph/spacebeforesizetype/) { get; set; } | Obtient et définit la quantité d'espace blanc vertical qui sera présent avant un paragraphe. |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Obtient l'index de départ des caractères. (Hérité de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [Stops](../../aspose.cells.drawing.texts/textparagraph/stops/) { get; } | Obtient la liste des tabulations. |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Renvoie les options de texte. (Hérité de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.texts/textparagraph/type/) { get; } | Obtient le type de nœud de texte. |

## Méthodes

| Nom | Description |
| --- | --- |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | Définit le style WordArt prédéfini.(Hérité de [`FontSetting`](../../aspose.cells/fontsetting/).) |

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter une zone de texte à la feuille de calcul
            int textBoxIndex = sheet.TextBoxes.Add(10, 10, 200, 100);
            Aspose.Cells.Drawing.TextBox textBox = sheet.TextBoxes[textBoxIndex];
            
            // Définit le contenu texte avec plusieurs paragraphes
            textBox.Text = "First paragraph\nSecond paragraph\nThird paragraph";

            // Accéder et modifier les paragraphes de texte
            foreach (TextParagraph paragraph in textBox.TextBody.TextParagraphs)
            {
                // Définir les propriétés du paragraphe
                paragraph.LineSpaceSizeType = LineSpaceSizeType.Points;
                paragraph.LineSpace = 20;
                paragraph.AlignmentType = TextAlignmentType.Center;
            }

            // Enregistrez le classeur
            workbook.Save("TextParagraphDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FontSetting](../../aspose.cells/fontsetting/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


