---
title: "Énumération TextVerticalType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.Drawing.Texts.TextVerticalType. Représente le type de direction du texte"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textverticaltype/
---
## TextVerticalType enumeration

Représente le type direct du texte.

```csharp
public enum TextVerticalType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Vertical | `0` | Affichage vertical est-asiatique. |
| Horizontal | `1` | Texte horizontal. |
| VerticalLeftToRight | `2` | Affiché verticalement et le texte s'écoule de haut en bas puis de GAUCHE à DROITE |
| Vertical90 | `3` | Chaque ligne est tournée de 90 degrés dans le sens des aiguilles d'une montre |
| Vertical270 | `4` | Chaque ligne est tournée de 270 degrés dans le sens des aiguilles d'une montre |
| Stacked | `5` | Détermine si tout le texte est vertical |
| StackedRightToLeft | `6` | Spécifie que le WordArt vertical doit être affiché de droite à gauche plutôt que de gauche à droite. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextVerticalTypeDemo
    {
        public static void TextVerticalTypeExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajout d'une forme rectangulaire à la feuille de calcul
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 50, 100);

            // Accéder aux paramètres d'alignement du texte de la forme
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;

            // Définir le type vertical du texte sur Horizontal
            shapeTextAlignment.TextVerticalType = TextVerticalType.Horizontal;

            // Définir d'autres propriétés à des fins de démonstration
            shapeTextAlignment.IsTextWrapped = true;
            shapeTextAlignment.RotateTextWithShape = true;
            shapeTextAlignment.TextVerticalOverflow = TextOverflowType.Clip;
            shapeTextAlignment.TextHorizontalOverflow = TextOverflowType.Clip;
            shapeTextAlignment.RotationAngle = 90;
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
            workbook.Save("TextVerticalTypeExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


