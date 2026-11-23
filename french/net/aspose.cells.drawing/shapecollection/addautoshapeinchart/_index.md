---
title: "ShapeCollection.AddAutoShapeInChart"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Ajoute une AutoShape au graphique"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/addautoshapeinchart/
---
## ShapeCollection.AddAutoShapeInChart method

Ajoute un AutoShape au graphique.

```csharp
public Shape AddAutoShapeInChart(AutoShapeType type, int top, int left, int height, int width)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | AutoShapeType | Type de forme automatique. |
| haut | Int32 | Représente le décalage vertical de la zone de texte depuis le coin supérieur gauche, en unités de 1/4000 de la zone du graphique. |
| gauche | Int32 | Représente le décalage vertical de la zone de texte depuis le coin supérieur gauche, en unités de 1/4000 de la zone du graphique. |
| hauteur | Int32 | Représente la hauteur de la zone de texte, en unités de 1/4000 de la zone du graphique. |
| largeur | Int32 | Représente la largeur de la zone de texte, en unités de 1/4000 de la zone du graphique. |

### Valeur de retour

Renvoie un objet forme.

### Remarques

Le type ne peut pas être Chart/Comment/Picture/OleObject/Polygon/DialogBox

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeCollectionMethodAddAutoShapeInChartWithAutoShapeTypeInt32Int32Int32InDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // Appelez la méthode AddAutoShapeInChart pour ajouter une forme étoile au graphique
                Shape shape = chart.Shapes.AddAutoShapeInChart(
                    AutoShapeType.Star16,  // AutoShapeType
                    100,                  // Top position (in pixels)
                    100,                  // Left position (in pixels)
                    200,                  // Height (in pixels)
                    200);                 // Width (in pixels)

                // Définir les propriétés de la forme
                shape.Name = "SampleStar";
                shape.Fill.SolidFill.Color = System.Drawing.Color.Yellow;
                shape.Line.SolidFill.Color = System.Drawing.Color.Red;

                Console.WriteLine("Star shape added successfully to the chart.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddAutoShapeInChart method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("ShapeCollectionMethodAddAutoShapeInChartDemo.xlsx");
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


