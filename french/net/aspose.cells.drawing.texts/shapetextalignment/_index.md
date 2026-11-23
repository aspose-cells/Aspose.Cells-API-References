---
title: "Classe ShapeTextAlignment"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.Texts.ShapeTextAlignment. Représente le paramètre d'alignement du texte des formes"
type: docs
url: /fr/net/aspose.cells.drawing.texts/shapetextalignment/
---
## ShapeTextAlignment class

Représente le paramètre d'alignement du texte de la forme ;

```csharp
public class ShapeTextAlignment
```

## Propriétés

| Nom | Description |
| --- | --- |
| [AutoSize](../../aspose.cells.drawing.texts/shapetextalignment/autosize/) { get; set; } | Indique si la taille de la forme est ajustée automatiquement en fonction de son contenu. |
| [BottomMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/bottommarginpt/) { get; set; } | Renvoie la marge inférieure en unités de points |
| [IsAutoMargin](../../aspose.cells.drawing.texts/shapetextalignment/isautomargin/) { get; set; } | Indique si la marge du cadre de texte est automatique. |
| [IsLockedText](../../aspose.cells.drawing.texts/shapetextalignment/islockedtext/) { get; set; } | Indique si la forme est verrouillée lorsque la feuille de calcul est protégée. |
| [IsTextWrapped](../../aspose.cells.drawing.texts/shapetextalignment/istextwrapped/) { get; set; } | Obtient ou définit le type d'enroulement du texte de la forme qui contient du texte. |
| [LeftMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/leftmarginpt/) { get; set; } | Renvoie la marge gauche en unités de points |
| [NumberOfColumns](../../aspose.cells.drawing.texts/shapetextalignment/numberofcolumns/) { get; set; } | Obtient et définit le nombre de colonnes de texte dans le rectangle englobant. |
| [RightMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/rightmarginpt/) { get; set; } | Renvoie la marge droite en unités de points |
| [RotateTextWithShape](../../aspose.cells.drawing.texts/shapetextalignment/rotatetextwithshape/) { get; set; } | Indique si le texte tourne avec la forme. |
| [RotationAngle](../../aspose.cells.drawing.texts/shapetextalignment/rotationangle/) { get; set; } | Obtient et définit la rotation de la forme. |
| [TextHorizontalOverflow](../../aspose.cells.drawing.texts/shapetextalignment/texthorizontaloverflow/) { get; set; } | Obtient et définit le type de dépassement horizontal du texte de la zone de texte. |
| [TextShapeType](../../aspose.cells.drawing.texts/shapetextalignment/textshapetype/) { get; set; } | Obtient et définit le type de transformation du texte. |
| [TextVerticalOverflow](../../aspose.cells.drawing.texts/shapetextalignment/textverticaloverflow/) { get; set; } | Obtient et définit le type de dépassement vertical du texte de la zone de texte. |
| [TextVerticalType](../../aspose.cells.drawing.texts/shapetextalignment/textverticaltype/) { get; set; } | Obtient et définit la direction du texte. |
| [TopMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/topmarginpt/) { get; set; } | Renvoie la marge supérieure en unités de points |

## Méthodes

| Nom | Description |
| --- | --- |
| override [Equals](../../aspose.cells.drawing.texts/shapetextalignment/equals/)(object) | Détermine si cette instance a la même valeur qu'un autre objet `ShapeTextAlignment` spécifié. |
| override [GetHashCode](../../aspose.cells.drawing.texts/shapetextalignment/gethashcode/)() |  |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class ShapeTextAlignmentDemo
    {
        public static void ShapeTextAlignmentExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajout d'une forme rectangulaire à la feuille de calcul
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 50, 100);

            // Accès à l'objet ShapeTextAlignment
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;

            // Définition des propriétés
            shapeTextAlignment.IsTextWrapped = true;
            shapeTextAlignment.RotateTextWithShape = true;
            shapeTextAlignment.TextVerticalOverflow = TextOverflowType.Clip;
            shapeTextAlignment.TextHorizontalOverflow = TextOverflowType.Clip;
            shapeTextAlignment.RotationAngle = 90;
            shapeTextAlignment.TextVerticalType = TextVerticalType.Horizontal;
            shapeTextAlignment.IsLockedText = false;
            shapeTextAlignment.AutoSize = false;
            shapeTextAlignment.TextShapeType = AutoShapeType.TextBox;
            shapeTextAlignment.TopMarginPt = 2.0d;
            shapeTextAlignment.BottomMarginPt = 2.0d;
            shapeTextAlignment.LeftMarginPt = 2.0d;
            shapeTextAlignment.RightMarginPt = 2.0d;
            shapeTextAlignment.IsAutoMargin = true;
            shapeTextAlignment.NumberOfColumns = 1;

            // Enregistrement du classeur
            workbook.Save("ShapeTextAlignmentExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


