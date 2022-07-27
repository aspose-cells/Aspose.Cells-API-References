---
title: FillFormat
second_title: Référence de l'API Aspose.Cells pour .NET
description: Encapsule lobjet qui représente la mise en forme de remplissage dune forme.
type: docs
weight: 1970
url: /fr/net/aspose.cells.drawing/fillformat/
---
## FillFormat class

Encapsule l'objet qui représente la mise en forme de remplissage d'une forme.

```csharp
public class FillFormat
```

## Propriétés

| Nom | La description |
| --- | --- |
| [FillType](../../aspose.cells.drawing/fillformat/filltype) { get; set; } | Obtient et définit le type de remplissage |
| [GradientColor1](../../aspose.cells.drawing/fillformat/gradientcolor1) { get; } | Renvoie la couleur de dégradé 1 pour le remplissage spécifié. |
| [GradientColor2](../../aspose.cells.drawing/fillformat/gradientcolor2) { get; } | Renvoie la couleur de dégradé 2 pour le remplissage spécifié. |
| [GradientColorType](../../aspose.cells.drawing/fillformat/gradientcolortype) { get; } | Renvoie le type de couleur de dégradé pour le remplissage spécifié. |
| [GradientDegree](../../aspose.cells.drawing/fillformat/gradientdegree) { get; } | Renvoie le degré de dégradé pour le remplissage spécifié. S'applique uniquement à Excel 2007. |
| [GradientFill](../../aspose.cells.drawing/fillformat/gradientfill) { get; } | Obtient[`GradientFill`](./gradientfill) objet. |
| [GradientStyle](../../aspose.cells.drawing/fillformat/gradientstyle) { get; } | Renvoie le style de dégradé pour le remplissage spécifié. |
| [GradientVariant](../../aspose.cells.drawing/fillformat/gradientvariant) { get; } | Renvoie la variante de dégradé pour le remplissage spécifié. S'applique uniquement à Excel 2007. |
| [ImageData](../../aspose.cells.drawing/fillformat/imagedata) { get; set; } | Obtient et définit les données d'image de l'image. |
| [Pattern](../../aspose.cells.drawing/fillformat/pattern) { get; set; } | Représente le modèle d'affichage d'une zone. |
| [PatternFill](../../aspose.cells.drawing/fillformat/patternfill) { get; } | Obtient[`PatternFill`](./patternfill) objet. |
| [PictureFormatType](../../aspose.cells.drawing/fillformat/pictureformattype) { get; set; } | Obtient et définit le type de format d'image. |
| [PresetColor](../../aspose.cells.drawing/fillformat/presetcolor) { get; } | Renvoie la couleur prédéfinie du dégradé pour le remplissage spécifié. |
| [Scale](../../aspose.cells.drawing/fillformat/scale) { get; set; } | Obtient et définit l'échelle du format d'image. |
| [SolidFill](../../aspose.cells.drawing/fillformat/solidfill) { get; } | Obtient[`SolidFill`](./solidfill) objet. |
| [Texture](../../aspose.cells.drawing/fillformat/texture) { get; set; } | Représente le type de texture pour le remplissage spécifié. |
| [TextureFill](../../aspose.cells.drawing/fillformat/texturefill) { get; } | Obtient[`TextureFill`](./texturefill) objet. |
| [Transparency](../../aspose.cells.drawing/fillformat/transparency) { get; set; } | Renvoie ou définit le degré de transparence de la zone sous la forme d'une valeur comprise entre 0,0 (opaque) et 1,0 (clair). |

## Méthodes

| Nom | La description |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fillformat/equals)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/fillformat/gethashcode)() | Obtient le code de hachage. |
| [SetOneColorGradient](../../aspose.cells.drawing/fillformat/setonecolorgradient)(Color, double, GradientStyleType, int) | Définit le remplissage spécifié sur un dégradé d'une seule couleur. S'applique uniquement à Excel 2007. |
| [SetPresetColorGradient](../../aspose.cells.drawing/fillformat/setpresetcolorgradient)(GradientPresetType, GradientStyleType, int) | Définit le remplissage spécifié sur un dégradé de couleurs prédéfinies. S'applique uniquement à Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient#settwocolorgradient_1)(Color, Color, GradientStyleType, int) | Définit le remplissage spécifié sur un dégradé bicolore. S'applique uniquement à Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient#settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | Définit le remplissage spécifié sur un dégradé bicolore. S'applique uniquement à Excel 2007. |

### Exemples

```csharp

[C#]

//Instanciation d'un objet Workbook
Workbook workbook = new Workbook();
//Ajout d'une nouvelle feuille de calcul à l'objet Excel
int sheetIndex = workbook.Worksheets.Add();
//Obtention de la référence de la feuille de calcul nouvellement ajoutée en passant son index de feuille
Worksheet worksheet = workbook.Worksheets[sheetIndex];
//Ajout d'un exemple de valeur à la cellule "A1"
worksheet.Cells["A1"].PutValue(50);
//Ajout d'un exemple de valeur à la cellule "A2"
worksheet.Cells["A2"].PutValue(100);
//Ajout d'un exemple de valeur à la cellule "A3"
worksheet.Cells["A3"].PutValue(150);
//Ajout d'un exemple de valeur à la cellule "A4"
worksheet.Cells["A4"].PutValue(200);
//Ajout d'un exemple de valeur à la cellule "B1"
worksheet.Cells["B1"].PutValue(60);
//Ajout d'un exemple de valeur à la cellule "B2"
worksheet.Cells["B2"].PutValue(32);
//Ajout d'un exemple de valeur à la cellule "B3"
worksheet.Cells["B3"].PutValue(50);
//Ajout d'un exemple de valeur à la cellule "B4"
worksheet.Cells["B4"].PutValue(40);
//Ajout d'un exemple de valeur à la cellule "C1" en tant que données de catégorie
worksheet.Cells["C1"].PutValue("Q1");
//Ajout d'un exemple de valeur à la cellule "C2" en tant que données de catégorie
worksheet.Cells["C2"].PutValue("Q2");
//Ajout d'un exemple de valeur à la cellule "C3" en tant que données de catégorie
worksheet.Cells["C3"].PutValue("Y1");
//Ajout d'un exemple de valeur à la cellule "C4" en tant que données de catégorie
worksheet.Cells["C4"].PutValue("Y2");
//Ajout d'un graphique à la feuille de calcul
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
//Accéder à l'instance du graphique nouvellement ajouté
Chart chart = worksheet.Charts[chartIndex];
//Ajout de NSeries (source de données du graphique) au graphique allant de la cellule "A1" à "B4"
int seriesIndex = chart.NSeries.Add("A1:B4", true);
//Définition de la source de données pour les données de catégorie de NSeries
chart.NSeries.CategoryData = "C1:C4";
//Remplissage de la zone de la 2nd NSeries avec un dégradé
chart.NSeries[seriesIndex].Area.FillFormat.SetOneColorGradient(Color.Lime, 1, GradientStyleType.Horizontal, 1);

[Visual Basic]

Instanciation d'un objet Workbook
Dim workbook As Workbook = New Workbook()
'Ajout d'une nouvelle feuille de calcul à l'objet Excel
Dim sheetIndex As Int32 = workbook.Worksheets.Add()
'Obtenir la référence de la feuille de calcul nouvellement ajoutée en passant son index de feuille
Dim worksheet As Worksheet = workbook.Worksheets(sheetIndex)
'Adding a sample value to "A1" cell
worksheet.Cells("A1").PutValue(50)
'Adding a sample value to "A2" cell
worksheet.Cells("A2").PutValue(100)
'Adding a sample value to "A3" cell
worksheet.Cells("A3").PutValue(150)
'Adding a sample value to "A4" cell
worksheet.Cells("A4").PutValue(200)
'Adding a sample value to "B1" cell
worksheet.Cells("B1").PutValue(60)
'Adding a sample value to "B2" cell
worksheet.Cells("B2").PutValue(32)
'Adding a sample value to "B3" cell
worksheet.Cells("B3").PutValue(50)
'Adding a sample value to "B4" cell
worksheet.Cells("B4").PutValue(40)
'Adding a sample value to "C1" cell as category data
worksheet.Cells("C1").PutValue("Q1")
'Adding a sample value to "C2" cell as category data
worksheet.Cells("C2").PutValue("Q2")
'Adding a sample value to "C3" cell as category data
worksheet.Cells("C3").PutValue("Y1")
'Adding a sample value to "C4" cell as category data
worksheet.Cells("C4").PutValue("Y2")
'Ajouter un graphique à la feuille de calcul
Dim chartIndex As Int32 = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)
'Accéder à l'instance du graphique nouvellement ajouté
Dim chart As Chart = worksheet.Charts(chartIndex)
'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
Dim seriesIndex As Int32 = chart.NSeries.Add("A1:B4", True)
'Définition de la source de données pour les données de catégorie de NSeries
chart.NSeries.CategoryData = "C1:C4"
'Remplir la zone de la 2e NSeries avec un dégradé
chart.NSeries(seriesIndex).Area.FillFormat.SetOneColorGradient(Color.Lime, 1, GradientStyleType.Horizontal, 1)
```

### Voir également

* espace de noms [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
