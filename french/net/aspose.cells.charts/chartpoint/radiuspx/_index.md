---
title: "ChartPoint.RadiusPx"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartPoint. Obtient le rayon du camembert à bulles ou du beignet en unités de pixels après les appels à la méthode Chart.Calculate."
type: docs
url: /fr/net/aspose.cells.charts/chartpoint/radiuspx/
---
## ChartPoint.RadiusPx property

Obtient le rayon de la bulle, du diagramme circulaire ou du diagramme en anneau en unités de pixels après les appels à la méthode Chart.Calculate().

```csharp
public int RadiusPx { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyRadiusPxDemo
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

            // Ajouter un graphique en secteurs
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calculer le graphique pour s'assurer que les propriétés sont renseignées
            chart.Calculate();

            // Obtenir le premier point du graphique
            ChartPoint point = chart.NSeries[0].Points[0];

            // Afficher la valeur actuelle du rayon
            Console.WriteLine("Current RadiusPx value: " + point.RadiusPx);

            // Remarque : RadiusPx est en lecture seule, nous ne pouvons donc pas le définir directement.
            // Pour modifier le rayon, nous devons ajuster la taille du graphique ou d'autres propriétés.
            // qui affectent la taille du point indirectement

            // Exemple de la façon dont la modification de la taille du graphique affecte le rayon
            Console.WriteLine("\nChanging chart size to demonstrate radius change...");
            chart.ChartObject.Width = 800;
            chart.ChartObject.Height = 600;
            chart.Calculate();

            // Afficher la nouvelle valeur du rayon après le redimensionnement du graphique
            Console.WriteLine("New RadiusPx value after chart resize: " + point.RadiusPx);

            // Enregistrer le résultat
            workbook.Save("ChartPointPropertyRadiusPxDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


