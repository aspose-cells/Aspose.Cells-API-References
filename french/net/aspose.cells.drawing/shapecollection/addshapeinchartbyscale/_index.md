---
title: "ShapeCollection.AddShapeInChartByScale"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Ajoute une forme au graphique. Toutes les unités sont en pourcentage de l'échelle de la zone du graphique"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/addshapeinchartbyscale/
---
## AddShapeInChartByScale(MsoDrawingType, PlacementType, double, double, double, double) {#addshapeinchartbyscale}

Ajoute une forme au graphique. Toutes les unités sont à l'échelle en pourcentage de la zone du graphique.

```csharp
public Shape AddShapeInChartByScale(MsoDrawingType type, PlacementType placement, double left, 
    double top, double right, double bottom)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | MsoDrawingType | Le type de dessin. |
| placement | PlacementType | le type de placement. |
| gauche | Double | L'unité est le pourcentage de l'échelle de la largeur de la zone du graphique. |
| haut | Double | L'unité est le pourcentage de l'échelle de la hauteur de la zone du graphique. |
| droite | Double | L'unité est le pourcentage de l'échelle de la largeur de la zone du graphique. |
| bas | Double | L'unité est le pourcentage de l'échelle de la hauteur de la zone du graphique. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddShapeInChartByScaleWithMsoDrawingTypePlacementTypeDouDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 1, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Calculer le graphique
            chart.Calculate();

            // Ajouter une forme rectangle au graphique en utilisant des coordonnées à l'échelle
            Shape rectangle = chart.Shapes.AddShapeInChartByScale(
                MsoDrawingType.Rectangle, 
                PlacementType.Move,
                0.2,  // x1 (20% from left)
                0.2,  // y1 (20% from top)
                0.4,  // x2 (40% from left)
                0.4); // y2 (40% from top)
            rectangle.Fill.SolidFill.Color = Color.Blue;
            rectangle.Line.SolidFill.Color = Color.Black;

            // Ajouter une forme ovale au graphique en utilisant des coordonnées à l'échelle
            Shape oval = chart.Shapes.AddShapeInChartByScale(
                MsoDrawingType.Oval,
                PlacementType.Move,
                0.6,  // x1 (60% from left)
                0.6,  // y1 (60% from top)
                0.8,  // x2 (80% from left)
                0.8); // y2 (80% from top)
            oval.Fill.SolidFill.Color = Color.Red;
            oval.Line.SolidFill.Color = Color.Black;

            // Enregistrez le classeur
            workbook.Save("AddShapeInChartByScaleWithMsoDrawingType.xlsx");
        }
    }
}
```

### Voir aussi

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* enum [PlacementType](../../placementtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## AddShapeInChartByScale(MsoDrawingType, PlacementType, double, double, double, double, byte[]) {#addshapeinchartbyscale_1}

Ajoute une forme au graphique. Toutes les unités sont 1/4000 de la zone du graphique.

```csharp
public Shape AddShapeInChartByScale(MsoDrawingType type, PlacementType placement, double left, 
    double top, double right, double bottom, byte[] imageData)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | MsoDrawingType | Le type de dessin. |
| placement | PlacementType | le type de placement. |
| gauche | Double | L'unité est le pourcentage de l'échelle de la largeur de la zone du graphique. |
| haut | Double | L'unité est le pourcentage de l'échelle de la hauteur de la zone du graphique. |
| droite | Double | L'unité est le pourcentage de l'échelle de la largeur de la zone du graphique. |
| bas | Double | L'unité est le pourcentage de l'échelle de la hauteur de la zone du graphique. |
| imageData | Byte[] | Si la forme n'est pas une image ou un objet OLE, imageData doit être nul. |

### Voir aussi

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* enum [PlacementType](../../placementtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


