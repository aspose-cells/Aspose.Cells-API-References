---
title: "Axis.CrossAt"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Axis. Représente le point sur l'axe des valeurs où l'axe des catégories le croise"
type: docs
url: /fr/net/aspose.cells.charts/axis/crossat/
---
## Axis.CrossAt property

Représente le point sur l'axe des valeurs où l'axe des catégories le croise.

```csharp
public double CrossAt { get; set; }
```

### Remarques

Le nombre doit être un entier lorsqu'il s'applique à l'axe des catégories. Et la valeur doit être comprise entre 1 et 31999.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyCrossAtDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["A5"].PutValue("D");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Configurer l'axe des valeurs
            chart.ValueAxis.CrossAt = 15; // Cross at value 15
            chart.ValueAxis.MinValue = 0;
            chart.ValueAxis.MaxValue = 50;

            // Configurer l'axe des catégories
            chart.CategoryAxis.CrossAt = 2.5; // Cross between categories B and C
            chart.CategoryAxis.TickLabelPosition = Aspose.Cells.Charts.TickLabelPositionType.Low;

            // Enregistrez le classeur
            workbook.Save("AxisCrossAtDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


