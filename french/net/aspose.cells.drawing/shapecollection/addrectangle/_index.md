---
title: "ShapeCollection.AddRectangle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Ajoute un RectangleShape à la feuille de calcul"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/addrectangle/
---
## ShapeCollection.AddRectangle method

Ajoute une forme rectangulaire à la feuille de calcul.

```csharp
public RectangleShape AddRectangle(int topRow, int top, int leftColumn, int left, int height, 
    int width)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Indice de la ligne supérieure gauche. |
| haut | Int32 | Représente le décalage vertical du RectangleShape depuis sa ligne de gauche, en unité de pixel. |
| leftColumn | Int32 | Indice de la colonne supérieure gauche. |
| gauche | Int32 | Représente le décalage horizontal de RectangleShape par rapport à sa colonne de gauche, en unité de pixel. |
| hauteur | Int32 | Représente la hauteur de RectangleShape, en unité de pixel. |
| largeur | Int32 | Représente la largeur de RectangleShape, en unité de pixel. |

### Valeur de retour

Un objet RectangleShape.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddRectangleWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un rectangle en utilisant les paramètres spécifiés
            RectangleShape rectangleShape = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 130, 130);

            // Enregistrez le classeur
            workbook.Save("RectangleShapeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [RectangleShape](../../rectangleshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


