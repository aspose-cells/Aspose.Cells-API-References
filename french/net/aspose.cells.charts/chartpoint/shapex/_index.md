---
title: "ChartPoint.ShapeX"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartPoint. Obtient la coordonnée x du coin supérieur gauche en unités de 1/4000 de la largeur du graphique après l'appel de la méthode Chart.Calculate."
type: docs
url: /fr/net/aspose.cells.charts/chartpoint/shapex/
---
## ChartPoint.ShapeX property

Obtient la coordonnée x du coin supérieur gauche en unités de 1/4000 de la largeur du graphique après l'appel de la méthode Chart.Calculate().

```csharp
public int ShapeX { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeXDemo
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

            // Ajouter un graphique en colonnes
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calculez le graphique pour vous assurer que ShapeX est renseigné.
            chart.Calculate();

            // Obtenir le premier point de la première série
            ChartPoint point = chart.NSeries[0].Points[0];

            // Affichez la valeur de ShapeX (1/4000 de la largeur du graphique).
            Console.WriteLine("ShapeX value (1/4000 units): " + point.ShapeX);
            Console.WriteLine("ShapeX value (pixels): " + point.ShapeXPx);

            // Démontrez l'utilisation de ShapeX pour positionner les éléments par rapport au point du graphique.
            // Remarque : comme ShapeX est en lecture seule, nous ne pouvons pas le modifier directement,
            // mais nous pouvons l'utiliser pour positionner d'autres éléments.
            if (point.ShapeX > 0)
            {
                // Ajoutez une zone de texte alignée avec la position X du point du graphique.
                Aspose.Cells.Drawing.TextBox textBox = worksheet.Shapes.AddTextBox(
                    point.ShapeXPx, 100, 100, 50, 100, 50);
                textBox.Text = "Point 1";
            }

            // Enregistrer le résultat
            workbook.Save("ChartPointShapeXDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


