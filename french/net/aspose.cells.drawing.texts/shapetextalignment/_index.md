---
title: ShapeTextAlignment
second_title: Référence de l'API Aspose.Cells pour .NET
description: Représente le paramètre dalignement du texte de la forme 
type: docs
weight: 2940
url: /fr/net/aspose.cells.drawing.texts/shapetextalignment/
---
## ShapeTextAlignment class

Représente le paramètre d'alignement du texte de la forme ;

```csharp
public class ShapeTextAlignment
```

## Propriétés

| Nom | La description |
| --- | --- |
| [AutoSize](../../aspose.cells.drawing.texts/shapetextalignment/autosize) { get; set; } | Indique si la taille de la forme est ajustée automatiquement en fonction de son contenu. |
| [BottomMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/bottommarginpt) { get; set; } | Renvoie la marge inférieure en unités de Points |
| [IsAutoMargin](../../aspose.cells.drawing.texts/shapetextalignment/isautomargin) { get; set; } | Indique si la marge du cadre de texte est automatique. |
| [IsTextWrapped](../../aspose.cells.drawing.texts/shapetextalignment/istextwrapped) { get; set; } | Obtient et définit le type de texte enveloppé de la forme qui contient du texte. |
| [LeftMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/leftmarginpt) { get; set; } | Renvoie la marge gauche en unité de Points |
| [RightMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/rightmarginpt) { get; set; } | Renvoie la marge droite en unité de Points |
| [RotateTextWithShape](../../aspose.cells.drawing.texts/shapetextalignment/rotatetextwithshape) { get; set; } | Indique si la rotation du texte avec la forme. |
| [RotationAngle](../../aspose.cells.drawing.texts/shapetextalignment/rotationangle) { get; set; } | Obtient et définit la rotation de la forme. |
| [TextHorizontalOverflow](../../aspose.cells.drawing.texts/shapetextalignment/texthorizontaloverflow) { get; set; } | Obtient et définit le type de débordement horizontal du texte de la zone de texte. |
| [TextShapeType](../../aspose.cells.drawing.texts/shapetextalignment/textshapetype) { get; set; } | Obtient et définit le type de transformation du texte. |
| [TextVerticalOverflow](../../aspose.cells.drawing.texts/shapetextalignment/textverticaloverflow) { get; set; } | Obtient et définit le type de débordement vertical du texte de la zone de texte. |
| [TextVerticalType](../../aspose.cells.drawing.texts/shapetextalignment/textverticaltype) { get; set; } | Obtient et définit la direction du texte. |
| [TopMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/topmarginpt) { get; set; } | Renvoie la marge supérieure en unités de Points |

## Méthodes

| Nom | La description |
| --- | --- |
| override [Equals](../../aspose.cells.drawing.texts/shapetextalignment/equals)(object) | Détermine si cette instance a la même valeur qu'une autre spécifiée[`ShapeTextAlignment`](../shapetextalignment) objet. |
| override [GetHashCode](../../aspose.cells.drawing.texts/shapetextalignment/gethashcode)() |  |

### Exemples

```csharp

[C#]
//Instanciation d'un objet Workbook
Workbook workbook = new Workbook();
Shape shape = workbook.Worksheets[0].Shapes.AddRectangle(1, 0, 1, 0, 50, 100);
Aspose.Cells.Drawing.Texts.ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;

//faites vos affaires

```

### Voir également

* espace de noms [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
