---
title: "ShapeCollection.AddLabelInChart"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Ajoute une étiquette au graphique"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/addlabelinchart/
---
## ShapeCollection.AddLabelInChart method

Ajoute une étiquette au graphique.

```csharp
public Label AddLabelInChart(int top, int left, int height, int width)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| haut | Int32 | Représente le décalage vertical de l'étiquette par rapport au coin supérieur gauche, en unités de 1/4000 de la zone du graphique. |
| gauche | Int32 | Représente le décalage vertical de l'étiquette par rapport au coin supérieur gauche, en unités de 1/4000 de la zone du graphique. |
| hauteur | Int32 | Représente la hauteur de l'étiquette, en unités de 1/4000 de la zone du graphique. |
| largeur | Int32 | Représente la largeur de l'étiquette, en unités de 1/4000 de la zone du graphique. |

### Valeur de retour

Un nouvel objet Label.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeCollectionMethodAddLabelInChartWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple pour créer un graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];            
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // Appelez la méthode AddLabelInChart avec les paramètres (top, left, height, width)
                Label label = chart.Shapes.AddLabelInChart(100, 100, 200, 200);
                
                // Définissez les propriétés de l'étiquette
                label.Text = "Sample Chart Label";
                label.Font.Color = System.Drawing.Color.Red;
                label.Font.Size = 12;

                Console.WriteLine("Label added successfully to chart with parameters (100, 100, 200, 50)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddLabelInChart method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("ShapeCollectionMethodAddLabelInChartWithInt32Int32Int32Int32Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Label](../../label/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


