---
title: "Classe Border"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Border classe. Encapsule l'objet qui représente la bordure de la cellule"
type: docs
url: /fr/net/aspose.cells/border/
---
## Border class

Encapsule l'objet qui représente la bordure de la cellule.

```csharp
public class Border
```

## Propriétés

| Nom | Description |
| --- | --- |
| [ArgbColor](../../aspose.cells/border/argbcolor/) { get; set; } | Obtient et définit la couleur avec une valeur ARGB 32 bits. |
| [Color](../../aspose.cells/border/color/) { get; set; } | Obtient ou définit la couleur de la bordure. |
| [LineStyle](../../aspose.cells/border/linestyle/) { get; set; } | Obtient ou définit le type de bordure de la cellule. |
| [ThemeColor](../../aspose.cells/border/themecolor/) { get; set; } | Obtient et définit la couleur de thème de la bordure. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class BorderDemo
    {
        public static void BorderExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();

            // Ajout d'une nouvelle feuille de calcul à l'objet Workbook
            workbook.Worksheets.Add();

            // Obtention de la référence de la feuille de calcul nouvellement ajoutée en passant son indice de feuille
            Worksheet worksheet = workbook.Worksheets[0];

            // Accès à la cellule "A1" de la feuille de calcul
            Cell cell = worksheet.Cells["A1"];

            // Ajout d'une valeur à la cellule "A1"
            cell.PutValue("Hello World");

            // Obtention du style de cellule
            Style style = cell.GetStyle();

            // Définition du style de ligne de la bordure supérieure
            Border topBorder = style.Borders[BorderType.TopBorder];
            topBorder.LineStyle = CellBorderType.Medium;
            topBorder.Color = Color.Red;

            // Définition du style de ligne de la bordure inférieure
            Border bottomBorder = style.Borders[BorderType.BottomBorder];
            bottomBorder.LineStyle = CellBorderType.Thick;
            bottomBorder.Color = Color.Blue;

            // Définition du style de ligne de la bordure gauche
            Border leftBorder = style.Borders[BorderType.LeftBorder];
            leftBorder.LineStyle = CellBorderType.Dashed;
            leftBorder.Color = Color.Green;

            // Définition du style de ligne de la bordure droite
            Border rightBorder = style.Borders[BorderType.RightBorder];
            rightBorder.LineStyle = CellBorderType.Dotted;
            rightBorder.Color = Color.Purple;

            // Appliquer le style à la cellule
            cell.SetStyle(style);

            // Enregistrement du fichier Excel
            workbook.Save("BorderExample.xlsx");
            workbook.Save("BorderExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


