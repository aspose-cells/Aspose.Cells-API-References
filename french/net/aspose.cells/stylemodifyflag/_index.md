---
title: "Enum StyleModifyFlag"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.StyleModifyFlag. Les indicateurs de style modifié"
type: docs
url: /fr/net/aspose.cells/stylemodifyflag/
---
## StyleModifyFlag enumeration

Les indicateurs de style modifié.

```csharp
public enum StyleModifyFlag
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| LeftBorder | `256` | Indique si la bordure gauche a été modifiée pour le style. |
| RightBorder | `512` | Indique si la bordure droite a été modifiée pour le style. |
| TopBorder | `1024` | Indique si la bordure supérieure a été modifiée pour le style. |
| BottomBorder | `2048` | Indique si la bordure inférieure a été modifiée pour le style. |
| DiagonalDownBorder | `4096` | Indique si la bordure diagonale descendante a été modifiée pour le style. |
| DiagonalUpBorder | `8192` | Indique si la bordure diagonale ascendante a été modifiée pour le style. |
| HorizontalBorder | `32` | Indique si la bordure horizontale a été modifiée pour le style. Seulement pour les styles dynamiques, tels que le formatage conditionnel. |
| VerticalBorder | `64` | Indique si la bordure verticale a été modifiée pour le style. Seulement pour les styles dynamiques, tels que le formatage conditionnel. |
| SideBorders | `3840` | Indique les bordures des quatre côtés : LeftBorder, RightBorder, TopBorder et BottomBorder. |
| Diagonal | `12288` | Indique les bordures diagonales : DiagonalDownBorder et DiagonalUpBorder. |
| DynamicStyleBorders | `96` | Indique les bordures du style dynamique : HorizontalBorder et VerticalBorder. |
| Borders | `16224` | Indique si une ou plusieurs bordures (LeftBorder, RightBorder, TopBorder, BottomBorder, Diagonal, HorizontalBorder, VerticalBorder) ont été modifiées pour le style. |
| NumberFormat | `16384` | Indique si numberformat a été modifié. |
| HorizontalAlignment | `32768` | Indique si l'alignement horizontal a été modifié. |
| VerticalAlignment | `65536` | Indique si l'alignement vertical a été modifié. |
| Indent | `131072` | Indique si la propriété d'indentation a été modifiée. |
| Rotation | `262144` | Indique si la propriété de rotation a été modifiée. |
| WrapText | `524288` | Indique si la propriété wrap text a été modifiée. |
| ShrinkToFit | `1048576` | Indique si la propriété réduire pour ajuster a été modifiée. |
| TextDirection | `2097152` | Indique si la propriété de direction du texte a été modifiée. |
| RelativeIndent | `128` | Indique si la propriété d'indentation relative a été modifiée pour le style. Uniquement pour les styles dynamiques, tels que le formatage conditionnel. |
| AlignmentSettings | `4161664` | Indique si une ou plusieurs propriétés liées à l'alignement (HorizontalAlignment, VerticalAlignment, Rotation, WrapText, WrapText, Indent, ShrinkToFit, TextDirection, RelativeIndent) ont été modifiées. |
| Pattern | `4194304` | Indique si le motif de l'ombrage a été modifié. |
| ForegroundColor | `8388608` | Indique si la couleur de premier plan a été modifiée. |
| BackgroundColor | `16777216` | Indique si la couleur d'arrière-plan a été modifiée. |
| CellShading | `29360128` | Indique si une ou plusieurs propriétés liées à l'ombrage (Pattern, ForegroundColor, BackgroundColor) ont été modifiées. |
| Locked | `67108864` | Indique si la propriété verrouillée a été modifiée. |
| HideFormula | `134217728` | Indique si hide formula a été modifié. |
| ProtectionSettings | `201326592` | Indique si une ou plusieurs propriétés liées à la protection (Locked, HideFormula) ont été modifiées. |
| FontSize | `1` | Indique si la taille de police a été modifiée. |
| FontName | `2` | Indique si le nom de police a été modifié. |
| FontColor | `3` | Indique si la couleur de police a été modifiée. |
| FontWeight | `4` | Indique si le poids de police a été modifié. |
| FontItalic | `5` | Indique si la propriété italique de la police a été modifiée. |
| FontUnderline | `6` | Indique si la propriété soulignée de la police a été modifiée. |
| FontStrike | `7` | Indique si la propriété barrée de la police a été modifiée. |
| FontScript | `8` | Indique si la propriété indice ou exposant de la police a été modifiée. |
| FontFamily | `9` | Indique si la famille de polices a été modifiée. |
| FontCharset | `10` | Indique si le jeu de caractères de la police a été modifié. |
| FontScheme | `11` | non utilisé. |
| FontDirty | `12` | non utilisé. |
| FontSpellingError | `13` | non utilisé. |
| FontUFillTx | `14` | non utilisé. |
| FontSpacing | `15` | non utilisé. |
| FontKerning | `16` | non utilisé. |
| FontEqualize | `17` | non utilisé. |
| FontCap | `18` | non utilisé. |
| FontVerticalText | `19` |  |
| Font | `31` | Indique si une ou plusieurs propriétés de la police du style ont été modifiées. |
| All | `234881023` | Toutes les propriétés pouvant être modifiées pour le style. |
| None | `0` | Aucune propriété n'a été spécifiée. |

### Remarques

Des combinaisons de plusieurs propriétés sont définies pour la commodité de l'utilisateur. Lors de la vérification de leur modification pour un style, la valeur retournée indique si une ou plusieurs propriétés de la combinaison ont été modifiées.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleModifyFlagDemo
    {
        public static void StyleModifyFlagExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir certaines valeurs dans la feuille de calcul
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["A2"].PutValue(123.45);

            // Créer un nouveau style
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.Color = System.Drawing.Color.Blue;
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;

            // Appliquer le style à une cellule
            worksheet.Cells["A1"].SetStyle(style);

            // Vérifier quelles propriétés du style ont été modifiées
            bool isFontModified = style.IsModified(StyleModifyFlag.Font);
            bool isFontSizeModified = style.IsModified(StyleModifyFlag.FontSize);
            bool isFontColorModified = style.IsModified(StyleModifyFlag.FontColor);
            bool isHorizontalAlignmentModified = style.IsModified(StyleModifyFlag.HorizontalAlignment);

            // Afficher les résultats
            Console.WriteLine("Font Modified: " + isFontModified);
            Console.WriteLine("Font Size Modified: " + isFontSizeModified);
            Console.WriteLine("Font Color Modified: " + isFontColorModified);
            Console.WriteLine("Horizontal Alignment Modified: " + isHorizontalAlignmentModified);

            // Enregistrez le classeur
            workbook.Save("StyleModifyFlagExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


