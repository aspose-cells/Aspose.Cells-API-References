---
title: "ChartPoint.YValueType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartPoint. Obtient le type de valeur Y du point du graphique."
type: docs
url: /fr/net/aspose.cells.charts/chartpoint/yvaluetype/
---
## ChartPoint.YValueType property

Obtient le type de valeur Y du point du graphique.

```csharp
public CellValueType YValueType { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyYValueTypeDemo
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

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtenir le premier point du graphique dans la première série
            ChartPoint chartPoint = chart.NSeries[0].Points[0];

            // Afficher le YValueType actuel.
            Console.WriteLine("Current YValueType: " + chartPoint.YValueType);

            // Afficher le YValue avant la modification
            Console.WriteLine("Current YValue: " + chartPoint.YValue);

            // Modifier le YValue en un type différent (string pour démontrer le changement de type)
            chartPoint.YValue = "15"; // This will change the YValueType to IsString

            // Afficher le YValueType après la modification
            Console.WriteLine("New YValueType: " + chartPoint.YValueType);
            Console.WriteLine("New YValue: " + chartPoint.YValue);

            // Enregistrez le classeur
            workbook.Save("ChartPointPropertyYValueTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [CellValueType](../../../aspose.cells/cellvaluetype/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


