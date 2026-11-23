---
title: "Enum BorderType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.BorderType enum. Énumère les types de lignes de bordure et de lignes diagonales"
type: docs
url: /fr/net/aspose.cells/bordertype/
---
## BorderType enumeration

Énumère les types de lignes de bordure et de lignes diagonales.

```csharp
[Flags]
public enum BorderType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| LeftBorder | `1` | Représente la ligne de bordure gauche. |
| RightBorder | `2` | Représente la ligne de bordure droite existante. |
| TopBorder | `4` | Représente la ligne de bordure supérieure. |
| BottomBorder | `8` | Représente la ligne de bordure inférieure. |
| DiagonalDown | `10` | Représente la ligne diagonale du coin supérieur gauche au coin inférieur droit. |
| DiagonalUp | `20` | Représente la ligne diagonale du coin inférieur gauche au coin supérieur droit. |
| Vertical | `40` | Uniquement pour le style dynamique, tel que le formatage conditionnel, le tableau croisé dynamique. |
| Horizontal | `80` | Uniquement pour le style dynamique, tel que le formatage conditionnel, le tableau croisé dynamique. |
| SideBorders | `F` | Indique les bordures des quatre côtés : LeftBorder, RightBorder, TopBorder et BottomBorder. |
| Diagonal | `30` | Combinaison spéciale de plusieurs bordures pour la commodité de l'utilisateur dans certaines API. Indique les bordures diagonales DiagonalUp et DiagonalDown. |
| DynamicStyleBorders | `C0` | Indique les bordures verticales et horizontales du style dynamique. |
| None | `0` | Aucune bordure n'a été spécifiée. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class BorderTypeDemo
    {
        public static void BorderTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            // Créer une plage de cellules
            var range = worksheet.Cells.CreateRange("A1:D4");

            // Créez un objet de style
            Style style = workbook.CreateStyle();
            // Définir les bordures pour la plage
            style.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.RightBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.TopBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.DiagonalDown, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.DiagonalUp, CellBorderType.Thin, Color.Blue);

            // Appliquer le style à la plage
            StyleFlag flag = new StyleFlag { Borders = true };
            range.ApplyStyle(style, flag);

            // Enregistrez le classeur
            workbook.Save("BorderTypeExample.xlsx");
            workbook.Save("BorderTypeExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


