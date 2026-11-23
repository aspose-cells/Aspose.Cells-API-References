---
title: "ShapeCollection.AddShapeInChart"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Ajoute une forme au graphique. Toutes les unités sont de 1/4000 de la zone du graphique"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/addshapeinchart/
---
## AddShapeInChart(MsoDrawingType, PlacementType, int, int, int, int, byte[]) {#addshapeinchart_1}

Ajoute une forme au graphique. Toutes les unités sont 1/4000 de la zone du graphique.

```csharp
public Shape AddShapeInChart(MsoDrawingType type, PlacementType placement, int left, int top, 
    int right, int bottom, byte[] imageData)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | MsoDrawingType | Le type de dessin. |
| placement | PlacementType | le type de placement. |
| gauche | Int32 | En unité de 1/4000 de la largeur de la zone du graphique. |
| haut | Int32 | En unité de 1/4000 de la hauteur de la zone du graphique. |
| droite | Int32 | En unité de 1/4000 de la largeur de la zone du graphique. |
| bas | Int32 | En unité de 1/4000 de la hauteur de la zone du graphique. |
| imageData | Byte[] | Si la forme n'est pas une image ou un objet OLE, imageData doit être nul. |

### Voir aussi

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* enum [PlacementType](../../placementtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## AddShapeInChart(MsoDrawingType, PlacementType, int, int, int, int) {#addshapeinchart}

Ajoute une forme au graphique. Toutes les unités sont 1/4000 de la zone du graphique.

```csharp
public Shape AddShapeInChart(MsoDrawingType type, PlacementType placement, int left, int top, 
    int right, int bottom)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | MsoDrawingType | Le type de dessin. |
| placement | PlacementType | le type de placement. |
| gauche | Int32 | En unité de 1/4000 de la largeur de la zone du graphique. |
| haut | Int32 | En unité de 1/4000 de la hauteur de la zone du graphique. |
| droite | Int32 | En unité de 1/4000 de la largeur de la zone du graphique. |
| bas | Int32 | En unité de 1/4000 de la hauteur de la zone du graphique. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddShapeInChartWithMsoDrawingTypePlacementTypeIntDemo
    {
        public static void Run()
        {
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Ajoutez une forme au graphique
            chart.Shapes.AddShapeInChart(MsoDrawingType.CheckBox, PlacementType.Move, 100, 100, 1000, 1000);
            
            // Définissez le texte de la forme
            chart.Shapes[0].Text = "Sample CheckBox";
            
            // Enregistrer le classeur
            workbook.Save("AddShapeInChartWithMsoDrawingType.xlsx");
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


