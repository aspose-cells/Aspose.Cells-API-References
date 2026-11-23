---
title: "ChartPoint.XValueType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartPoint. Obtient le type de valeur X du point du diagramme"
type: docs
url: /fr/net/aspose.cells.charts/chartpoint/xvaluetype/
---
## ChartPoint.XValueType property

Obtient le type de valeur X du point du graphique.

```csharp
public CellValueType XValueType { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyXValueTypeDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtenir le premier point du graphique
            ChartPoint point = chart.NSeries[0].Points[0];

            // Afficher le XValueType actuel
            Console.WriteLine("Current XValueType: " + point.XValueType);

            // Définir une nouvelle XValue (cela mettra automatiquement à jour le XValueType)
            point.XValue = DateTime.Now; // Changing to DateTime type
            Console.WriteLine("After setting DateTime value, XValueType: " + point.XValueType);

            point.XValue = "New Category"; // Changing to String type
            Console.WriteLine("After setting String value, XValueType: " + point.XValueType);

            point.XValue = 123.45; // Changing to Numeric type
            Console.WriteLine("After setting Numeric value, XValueType: " + point.XValueType);

            // Enregistrez le classeur
            workbook.Save("ChartPointXValueTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [CellValueType](../../../aspose.cells/cellvaluetype/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


