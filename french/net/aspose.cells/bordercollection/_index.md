---
title: BorderCollection
second_title: Référence de l'API Aspose.Cells pour .NET
description: Encapsule une collection deBorder./border objets.
type: docs
weight: 150
url: /fr/net/aspose.cells/bordercollection/
---
## BorderCollection class

Encapsule une collection de[`Border`](../border) objets.

```csharp
public class BorderCollection
```

## Propriétés

| Nom | La description |
| --- | --- |
| [DiagonalColor](../../aspose.cells/bordercollection/diagonalcolor) { get; set; } | Obtient ou définit leColor de lignes diagonales. |
| [DiagonalStyle](../../aspose.cells/bordercollection/diagonalstyle) { get; set; } | Obtient ou définit le style des lignes diagonales. |
| [Item](../../aspose.cells/bordercollection/item) { get; } | Obtient le[`Border`](../border) élément à l'index spécifié. |

## Méthodes

| Nom | La description |
| --- | --- |
| [SetColor](../../aspose.cells/bordercollection/setcolor)(Color) | Définit leColor de toutes les bordures de la collection. |
| [SetStyle](../../aspose.cells/bordercollection/setstyle)(CellBorderType) | Définit le style de toutes les bordures de la collection. |

### Exemples

```csharp

[C#]

//Instanciation d'un objet Workbook
Workbook workbook = new Workbook();

//Ajout d'une nouvelle feuille de calcul à l'objet Excel
workbook.Worksheets.Add();

//Obtention de la référence de la feuille de calcul nouvellement ajoutée en passant son index de feuille
Worksheet worksheet = workbook.Worksheets[0];

//Accéder à la cellule "A1" depuis la feuille de calcul
Cell cell = worksheet.Cells["A1"];

//Ajout d'une valeur à la cellule "A1"
cell.PutValue("Visit Aspose!");

Style style = cell.GetStyle();

//Définition du style de ligne de la bordure supérieure
style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;

//Définition de la couleur de la bordure supérieure
style.Borders[BorderType.TopBorder].Color = Color.Black;

//Définition du style de ligne de la bordure inférieure
style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thick;

//Définition de la couleur de la bordure inférieure
style.Borders[BorderType.BottomBorder].Color = Color.Black;

//Définition du style de ligne de la bordure gauche
style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thick;

//Définition de la couleur de la bordure gauche
style.Borders[BorderType.LeftBorder].Color = Color.Black;

//Définition du style de ligne de la bordure droite
style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thick;

//Définition de la couleur de la bordure droite
style.Borders[BorderType.RightBorder].Color = Color.Black;

cell.SetStyle(style);

//Enregistrement du fichier Excel
workbook.Save("book1.xls");

[VB.NET]

'Instanciation d'un objet Workbook
Dim workbook As Workbook = New Workbook()

'Ajout d'une nouvelle feuille de calcul à l'objet Workbook
workbook.Worksheets.Add()

'Obtenir la référence de la feuille de calcul nouvellement ajoutée en passant son index de feuille
Dim worksheet As Worksheet = workbook.Worksheets(0)

'Accessing the "A1" cell from the worksheet
Dim cell As Cell = worksheet.Cells("A1")

'Adding some value to the "A1" cell
cell.PutValue("Visit Aspose!")

Dim style as Style = cell.GetStyle()

'Définition du style de ligne de la bordure supérieure
style.Borders(BorderType.TopBorder).LineStyle = CellBorderType.Thick

'Définir la couleur de la bordure supérieure
style.Borders(BorderType.TopBorder).Color = Color.Black

'Définition du style de ligne de la bordure inférieure
style.Borders(BorderType.BottomBorder).LineStyle = CellBorderType.Thick

'Définir la couleur de la bordure inférieure
style.Borders(BorderType.BottomBorder).Color = Color.Black

'Définition du style de ligne de la bordure gauche
style.Borders(BorderType.LeftBorder).LineStyle = CellBorderType.Thick

'Définir la couleur de la bordure gauche
style.Borders(BorderType.LeftBorder).Color = Color.Black

'Définition du style de ligne de la bordure droite
style.Borders(BorderType.RightBorder).LineStyle = CellBorderType.Thick

'Définir la couleur de la bordure droite
style.Borders(BorderType.RightBorder).Color = Color.Black

cell.SetStyle(style)

'Enregistrement du fichier Excel
workbook.Save("book1.xls")
```

### Voir également

* espace de noms [Aspose.Cells](../../aspose.cells)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
