---
title: "Classe BorderCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.BorderCollection. Encapsule une collection d'objets Border"
type: docs
url: /fr/net/aspose.cells/bordercollection/
---
## BorderCollection class

Encapsule une collection d'objets [`Border`](../border/).

```csharp
public class BorderCollection
```

## Propriétés

| Nom | Description |
| --- | --- |
| [DiagonalColor](../../aspose.cells/bordercollection/diagonalcolor/) { get; set; } | Obtient ou définit la Couleur des lignes Diagonales. |
| [DiagonalStyle](../../aspose.cells/bordercollection/diagonalstyle/) { get; set; } | Obtient ou définit le style des lignes Diagonales. |
| [IsOutline](../../aspose.cells/bordercollection/isoutline/) { get; set; } | Indique si les bordures gauche, droite, supérieure et inférieure doivent être appliquées uniquement aux bordures extérieures d'une plage de cellules. La valeur par défaut est true. |
| [Item](../../aspose.cells/bordercollection/item/) { get; } | Obtient l'élément [`Border`](../border/) à l'index spécifié. |

## Méthodes

| Nom | Description |
| --- | --- |
| [SetColor](../../aspose.cells/bordercollection/setcolor/)(Color) | Définit la Couleur de toutes les bordures de la collection. |
| [SetStyle](../../aspose.cells/bordercollection/setstyle/)(CellBorderType) | Définit le style de toutes les bordures de la collection. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class BorderCollectionDemo
    {
        public static void BorderCollectionExample()
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
            cell.PutValue("Visit Aspose!");

            // Obtention du style de la cellule
            Style style = cell.GetStyle();

            // Définition du style de ligne de la bordure supérieure
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;

            // Définition de la couleur de la bordure supérieure
            style.Borders[BorderType.TopBorder].Color = Color.Red;

            // Définition du style de ligne de la bordure inférieure
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thick;

            // Définition de la couleur de la bordure inférieure
            style.Borders[BorderType.BottomBorder].Color = Color.Green;

            // Définition du style de ligne de la bordure gauche
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dashed;

            // Définition de la couleur de la bordure gauche
            style.Borders[BorderType.LeftBorder].Color = Color.Yellow;

            // Définition du style de ligne de la bordure droite
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Dotted;

            // Définition de la couleur de la bordure droite
            style.Borders[BorderType.RightBorder].Color = Color.Blue;

            // Définition des propriétés diagonales
            style.Borders.DiagonalColor = Color.Red;
            style.Borders.DiagonalStyle = CellBorderType.Dashed;

            // Appliquer le style à la cellule
            cell.SetStyle(style);

            // Enregistrement du fichier Excel
            workbook.Save("BorderCollectionExample.xlsx");
            workbook.Save("BorderCollectionExample.pdf");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


