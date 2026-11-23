---
title: "Classe FillFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.FillFormat. Encapsule l'objet qui représente le format de remplissage d'une forme"
type: docs
url: /fr/net/aspose.cells.drawing/fillformat/
---
## FillFormat class

Encapsule l'objet qui représente le format de remplissage d'une forme.

```csharp
public class FillFormat
```

## Propriétés

| Nom | Description |
| --- | --- |
| [FillType](../../aspose.cells.drawing/fillformat/filltype/) { get; set; } | Obtient et définit le type de remplissage |
| [GradientColor1](../../aspose.cells.drawing/fillformat/gradientcolor1/) { get; } | Renvoie la couleur de dégradé 1 pour le remplissage spécifié. |
| [GradientColor2](../../aspose.cells.drawing/fillformat/gradientcolor2/) { get; } | Renvoie la couleur de dégradé 2 pour le remplissage spécifié. |
| [GradientColorType](../../aspose.cells.drawing/fillformat/gradientcolortype/) { get; } | Renvoie le type de couleur de dégradé pour le remplissage spécifié. |
| [GradientDegree](../../aspose.cells.drawing/fillformat/gradientdegree/) { get; } | Renvoie le degré du dégradé pour le remplissage spécifié. S'applique uniquement à Excel 2007. |
| [GradientFill](../../aspose.cells.drawing/fillformat/gradientfill/) { get; } | Obtient l'objet [`GradientFill`](./gradientfill/). |
| [GradientStyle](../../aspose.cells.drawing/fillformat/gradientstyle/) { get; } | Renvoie le style du dégradé pour le remplissage spécifié. |
| [GradientVariant](../../aspose.cells.drawing/fillformat/gradientvariant/) { get; } | Renvoie la variante du dégradé pour le remplissage spécifié. S'applique uniquement à Excel 2007. |
| [ImageData](../../aspose.cells.drawing/fillformat/imagedata/) { get; set; } | Obtient et définit les données d'image. |
| [Pattern](../../aspose.cells.drawing/fillformat/pattern/) { get; set; } | Représente le motif d'affichage d'une zone. |
| [PatternFill](../../aspose.cells.drawing/fillformat/patternfill/) { get; } | Obtient l'objet [`PatternFill`](./patternfill/). |
| [PictureFormatType](../../aspose.cells.drawing/fillformat/pictureformattype/) { get; set; } | Obtient et définit le type de format d'image. |
| [PresetColor](../../aspose.cells.drawing/fillformat/presetcolor/) { get; } | Renvoie la couleur prédéfinie du dégradé pour le remplissage spécifié. |
| [Scale](../../aspose.cells.drawing/fillformat/scale/) { get; set; } | Obtient et définit l'échelle du format d'image. |
| [SetType](../../aspose.cells.drawing/fillformat/settype/) { get; set; } | (**Obsolète.**) Obtient le type de format de remplissage. |
| [SolidFill](../../aspose.cells.drawing/fillformat/solidfill/) { get; } | Obtient l'objet [`SolidFill`](./solidfill/). |
| [Texture](../../aspose.cells.drawing/fillformat/texture/) { get; set; } | Représente le type de texture pour le remplissage spécifié. |
| [TextureFill](../../aspose.cells.drawing/fillformat/texturefill/) { get; } | Obtient l'objet [`TextureFill`](./texturefill/). |
| [Transparency](../../aspose.cells.drawing/fillformat/transparency/) { get; set; } | Renvoie ou définit le degré de transparence de la zone comme une valeur de 0,0 (opaque) à 1,0 (transparent). |
| [Type](../../aspose.cells.drawing/fillformat/type/) { get; set; } | (**Obsolète.**) Obtient et définit le type de remplissage. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fillformat/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/fillformat/gethashcode/)() | Obtient le code de hachage. |
| [SetOneColorGradient](../../aspose.cells.drawing/fillformat/setonecolorgradient/)(Color, double, GradientStyleType, int) | Définit le remplissage spécifié comme un dégradé à une couleur. S'applique uniquement à Excel 2007. |
| [SetPresetColorGradient](../../aspose.cells.drawing/fillformat/setpresetcolorgradient/)(GradientPresetType, GradientStyleType, int) | Définit le remplissage spécifié comme un dégradé à couleur prédéfinie. S'applique uniquement à Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient/#settwocolorgradient_1)(Color, Color, GradientStyleType, int) | Définit le remplissage spécifié comme un dégradé à deux couleurs. S'applique uniquement à Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient/#settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | Définit le remplissage spécifié comme un dégradé à deux couleurs. S'applique uniquement à Excel 2007. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassFillFormatDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");
            
            // Ajoutez un graphique en colonnes à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ajouter une série de données au graphique
            int seriesIndex = chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";
            
            // Appliquer le remplissage en dégradé à la zone de série
            chart.NSeries[seriesIndex].Area.FillFormat.SetOneColorGradient(System.Drawing.Color.Lime, 1, 
                GradientStyleType.Horizontal, 1);
            
            // Enregistrez le classeur
            workbook.Save("FillFormatDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


