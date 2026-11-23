---
title: "ShapeCollection.AddArc"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Ajoute un ArcShape à la feuille de calcul"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/addarc/
---
## ShapeCollection.AddArc method

Ajoute un ArcShape à la feuille de calcul.

```csharp
public ArcShape AddArc(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Indice de la ligne supérieure gauche. |
| haut | Int32 | Représente le décalage vertical de ArcShape par rapport à sa ligne de gauche, en unité de pixel. |
| leftColumn | Int32 | Indice de la colonne supérieure gauche. |
| gauche | Int32 | Représente le décalage horizontal de ArcShape par rapport à sa colonne de gauche, en unité de pixel. |
| hauteur | Int32 | Représente la hauteur de ArcShape, en unité de pixel. |
| largeur | Int32 | Représente la largeur de ArcShape, en unité de pixel. |

### Valeur de retour

Un objet ArcShape.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddArcWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ShapeCollection shapes = worksheet.Shapes;
            ArcShape arcShape = shapes.AddArc(10, 10, 100, 50, 45, 180);
            
            workbook.Save("AddArcDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ArcShape](../../arcshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


