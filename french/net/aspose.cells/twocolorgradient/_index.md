---
title: "Classe TwoColorGradient"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.TwoColorGradient. Représente un dégradé à deux couleurs"
type: docs
url: /fr/net/aspose.cells/twocolorgradient/
---
## TwoColorGradient class

Représente un dégradé à deux couleurs.

```csharp
public class TwoColorGradient
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [TwoColorGradient](twocolorgradient/)(Color, Color, GradientStyleType, int) |  |

## Propriétés

| Nom | Description |
| --- | --- |
| [Color1](../../aspose.cells/twocolorgradient/color1/) { get; set; } | Obtient et définit la première couleur du dégradé. |
| [Color2](../../aspose.cells/twocolorgradient/color2/) { get; set; } | Obtient et définit la deuxième couleur du dégradé. |
| [GradientStyleType](../../aspose.cells/twocolorgradient/gradientstyletype/) { get; set; } | Obtient et définit le style d'ombrage du dégradé. |
| [Variant](../../aspose.cells/twocolorgradient/variant/) { get; set; } | Obtient et définit la variante du dégradé. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class CellsClassTwoColorGradientDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Initialiser TwoColorGradient avec les paramètres du constructeur
            TwoColorGradient gradient = new TwoColorGradient(
                Color.LightSkyBlue, 
                Color.DarkBlue, 
                GradientStyleType.DiagonalUp, 
                2);

            // Modifier les propriétés du dégradé après l'initialisation
            gradient.GradientStyleType = GradientStyleType.DiagonalDown;

            // Créer un style de cellule et appliquer le dégradé
            Style style = workbook.CreateStyle();
            style.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);

            // Appliquer le style à la cellule et ajouter du contenu
            Cell cell = worksheet.Cells["B2"];
            cell.PutValue("Aspose.Cells TwoColorGradient Demo");
            cell.SetStyle(style);

            // Ajuster les dimensions de la cellule pour la visibilité
            worksheet.Cells.SetRowHeight(1, 45);
            worksheet.Cells.SetColumnWidth(1, 55);

            // Enregistrer le résultat avec le formatage du dégradé
            workbook.Save("TwoColorGradientDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


