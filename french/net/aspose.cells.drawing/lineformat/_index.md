---
title: LineFormat
second_title: Référence de l'API Aspose.Cells pour .NET
description: Représente tous les paramètres de la ligne.
type: docs
weight: 2220
url: /fr/net/aspose.cells.drawing/lineformat/
---
## LineFormat class

Représente tous les paramètres de la ligne.

```csharp
public class LineFormat : FillFormat
```

## Propriétés

| Nom | La description |
| --- | --- |
| [BeginArrowheadLength](../../aspose.cells.drawing/lineformat/beginarrowheadlength) { get; set; } | Obtient et définit le type de longueur de la flèche de début de la ligne. |
| [BeginArrowheadStyle](../../aspose.cells.drawing/lineformat/beginarrowheadstyle) { get; set; } | Obtient et définit le type de flèche de début de la ligne. |
| [BeginArrowheadWidth](../../aspose.cells.drawing/lineformat/beginarrowheadwidth) { get; set; } | Obtient et définit le type de largeur de flèche de début de la ligne. |
| [CapType](../../aspose.cells.drawing/lineformat/captype) { get; set; } | Spécifie les majuscules de fin. |
| [CompoundType](../../aspose.cells.drawing/lineformat/compoundtype) { get; set; } | Spécifie le type composé de ligne. |
| [DashStyle](../../aspose.cells.drawing/lineformat/dashstyle) { get; set; } | Spécifie le type de tiret de ligne. |
| [EndArrowheadLength](../../aspose.cells.drawing/lineformat/endarrowheadlength) { get; set; } | Obtient et définit le type de longueur de la flèche de fin de la ligne. |
| [EndArrowheadStyle](../../aspose.cells.drawing/lineformat/endarrowheadstyle) { get; set; } | Obtient et définit le type de flèche de fin de la ligne. |
| [EndArrowheadWidth](../../aspose.cells.drawing/lineformat/endarrowheadwidth) { get; set; } | Obtient et définit le type de largeur de flèche de fin de la ligne. |
| [FillType](../../aspose.cells.drawing/fillformat/filltype) { get; set; } | Obtient et définit le type de remplissage |
| [GradientColor1](../../aspose.cells.drawing/fillformat/gradientcolor1) { get; } | Renvoie la couleur de dégradé 1 pour le remplissage spécifié. |
| [GradientColor2](../../aspose.cells.drawing/fillformat/gradientcolor2) { get; } | Renvoie la couleur de dégradé 2 pour le remplissage spécifié. |
| [GradientColorType](../../aspose.cells.drawing/fillformat/gradientcolortype) { get; } | Renvoie le type de couleur de dégradé pour le remplissage spécifié. |
| [GradientDegree](../../aspose.cells.drawing/fillformat/gradientdegree) { get; } | Renvoie le degré de dégradé pour le remplissage spécifié. S'applique uniquement à Excel 2007. |
| [GradientFill](../../aspose.cells.drawing/fillformat/gradientfill) { get; } | Obtient[`GradientFill`](../fillformat/gradientfill) objet. |
| [GradientStyle](../../aspose.cells.drawing/fillformat/gradientstyle) { get; } | Renvoie le style de dégradé pour le remplissage spécifié. |
| [GradientVariant](../../aspose.cells.drawing/fillformat/gradientvariant) { get; } | Renvoie la variante de dégradé pour le remplissage spécifié. S'applique uniquement à Excel 2007. |
| [ImageData](../../aspose.cells.drawing/fillformat/imagedata) { get; set; } | Obtient et définit les données d'image de l'image. |
| [JoinType](../../aspose.cells.drawing/lineformat/jointype) { get; set; } | Spécifie le type de jointure de ligne. |
| [Pattern](../../aspose.cells.drawing/fillformat/pattern) { get; set; } | Représente le modèle d'affichage d'une zone. |
| [PatternFill](../../aspose.cells.drawing/fillformat/patternfill) { get; } | Obtient[`PatternFill`](../fillformat/patternfill) objet. |
| [PictureFormatType](../../aspose.cells.drawing/fillformat/pictureformattype) { get; set; } | Obtient et définit le type de format d'image. |
| [PresetColor](../../aspose.cells.drawing/fillformat/presetcolor) { get; } | Renvoie la couleur prédéfinie du dégradé pour le remplissage spécifié. |
| [Scale](../../aspose.cells.drawing/fillformat/scale) { get; set; } | Obtient et définit l'échelle du format d'image. |
| [SolidFill](../../aspose.cells.drawing/fillformat/solidfill) { get; } | Obtient[`SolidFill`](../fillformat/solidfill) objet. |
| [Texture](../../aspose.cells.drawing/fillformat/texture) { get; set; } | Représente le type de texture pour le remplissage spécifié. |
| [TextureFill](../../aspose.cells.drawing/fillformat/texturefill) { get; } | Obtient[`TextureFill`](../fillformat/texturefill) objet. |
| [Transparency](../../aspose.cells.drawing/fillformat/transparency) { get; set; } | Renvoie ou définit le degré de transparence de la zone sous la forme d'une valeur comprise entre 0,0 (opaque) et 1,0 (clair). |
| [Weight](../../aspose.cells.drawing/lineformat/weight) { get; set; } | Obtient ou définit le poids de la ligne en unités de points. |

## Méthodes

| Nom | La description |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/lineformat/equals)(object) | Détermine si cette instance a la même valeur qu'une autre spécifiée[`LineFormat`](../lineformat) objet. |
| override [GetHashCode](../../aspose.cells.drawing/lineformat/gethashcode)() | Obtient le code de hachage. |
| [SetOneColorGradient](../../aspose.cells.drawing/fillformat/setonecolorgradient)(Color, double, GradientStyleType, int) | Définit le remplissage spécifié sur un dégradé d'une seule couleur. S'applique uniquement à Excel 2007. |
| [SetPresetColorGradient](../../aspose.cells.drawing/fillformat/setpresetcolorgradient)(GradientPresetType, GradientStyleType, int) | Définit le remplissage spécifié sur un dégradé de couleurs prédéfinies. S'applique uniquement à Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient)(Color, Color, GradientStyleType, int) | Définit le remplissage spécifié sur un dégradé bicolore. S'applique uniquement à Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | Définit le remplissage spécifié sur un dégradé bicolore. S'applique uniquement à Excel 2007. |

### Exemples

```csharp

[C#]
//Instanciation d'un objet Workbook
Workbook workbook = new Workbook();
ShapeCollection shapes = workbook.Worksheets[0].Shapes;
Shape shape = shapes.AddRectangle(1, 0, 1, 0, 50, 100);
LineFormat lineFmt = shape.Line;

//faites vos affaires

```

### Voir également

* class [FillFormat](../fillformat)
* espace de noms [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
