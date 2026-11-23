---
title: "ShapeCollection.AddAutoShape"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Ajoute une AutoShape à la feuille de calcul"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/addautoshape/
---
## ShapeCollection.AddAutoShape method

Ajoute un AutoShape à la feuille de calcul.

```csharp
public Shape AddAutoShape(AutoShapeType type, int topRow, int top, int leftColumn, int left, 
    int height, int width)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | AutoShapeType | Type de forme automatique. |
| topRow | Int32 | Indice de la ligne supérieure gauche. |
| haut | Int32 | Représente le décalage vertical de Shape par rapport à sa ligne de gauche, en unité de pixel. |
| leftColumn | Int32 | Indice de la colonne supérieure gauche. |
| gauche | Int32 | Représente le décalage horizontal de Shape par rapport à sa colonne de gauche, en unité de pixel. |
| hauteur | Int32 | Représente la hauteur de Shape, en unité de pixel. |
| largeur | Int32 | Représente la largeur de Shape, en unité de pixel. |

### Valeur de retour

Un objet Shape.

### Remarques

Le type ne peut pas être Chart/Comment/Picture/OleObject/Polygon/DialogBox

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddAutoShapeWithAutoShapeTypeInt32Int32Int32InDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ShapeCollection shapes = worksheet.Shapes;
            Shape autoShape = shapes.AddAutoShape(AutoShapeType.Cube, 1, 0, 1, 0, 100, 50);
            
            workbook.Save("AutoShapeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Shape](../../shape/)
* enum [AutoShapeType](../../autoshapetype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


