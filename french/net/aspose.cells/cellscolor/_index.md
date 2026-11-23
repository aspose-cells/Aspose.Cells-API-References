---
title: "Classe CellsColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.CellsColor. Représente tous les types de couleur"
type: docs
url: /fr/net/aspose.cells/cellscolor/
---
## CellsColor class

Représente tous les types de couleur.

```csharp
public class CellsColor
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Argb](../../aspose.cells/cellscolor/argb/) { get; set; } | Obtient et définit la couleur à partir d'une valeur ARGB de 32 bits. |
| [Color](../../aspose.cells/cellscolor/color/) { get; set; } | Obtient et définit la couleur RVB. |
| [ColorIndex](../../aspose.cells/cellscolor/colorindex/) { get; set; } | Obtient et définit l'index de couleur dans la palette. S'applique uniquement aux couleurs indexées. |
| [IsShapeColor](../../aspose.cells/cellscolor/isshapecolor/) { get; set; } | Obtient et définit la couleur qui doit être appliquée à la cellule ou à la forme. |
| [ThemeColor](../../aspose.cells/cellscolor/themecolor/) { get; set; } | Obtient la couleur du thème. S'applique uniquement au type de couleur de thème. |
| [Transparency](../../aspose.cells/cellscolor/transparency/) { get; set; } | Obtient et définit la transparence sous forme d'une valeur de 0,0 (opaque) à 1,0 (transparent). |
| [Type](../../aspose.cells/cellscolor/type/) { get; } | Le type de couleur. |

## Méthodes

| Nom | Description |
| --- | --- |
| [SetTintOfShapeColor](../../aspose.cells/cellscolor/settintofshapecolor/)(double) | Définir la teinte de la couleur de la forme |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellsColorDemo
    {
        public static void CellsColorExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une plage de cellules
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "A10");

            // Créer une instance de CellsColor
            CellsColor cellsColor = workbook.CreateCellsColor();

            // Définir les propriétés de CellsColor
            cellsColor.IsShapeColor = false;
            cellsColor.Color = Color.Red;
            cellsColor.ColorIndex = 5;
            cellsColor.Argb = Color.Blue.ToArgb();
            cellsColor.Transparency = 0.5;

            // Appliquer le CellsColor à la plage
            Style style = workbook.CreateStyle();
            style.ForegroundColor = cellsColor.Color;
            style.Pattern = BackgroundType.Solid;
            range.ApplyStyle(style, new StyleFlag { CellShading = true });

            // Enregistrez le classeur
            workbook.Save("CellsColorExample.xlsx");
            workbook.Save("CellsColorExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


