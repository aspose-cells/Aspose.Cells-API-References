---
title: "Axis.IsAutomaticMaxValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Axis. Indique si la valeur maximale est attribuée automatiquement"
type: docs
url: /fr/net/aspose.cells.charts/axis/isautomaticmaxvalue/
---
## Axis.IsAutomaticMaxValue property

Indique si la valeur maximale est attribuée automatiquement.

```csharp
public bool IsAutomaticMaxValue { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsAutomaticMaxValueDemo
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
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtenir l'axe des valeurs
            Axis valueAxis = chart.ValueAxis;

            // Démontrer la propriété IsAutomaticMaxValue
            Console.WriteLine("Initial IsAutomaticMaxValue: " + valueAxis.IsAutomaticMaxValue);
            Console.WriteLine("Initial MaxValue: " + valueAxis.MaxValue);

            // Désactiver la valeur maximale automatique et définir une valeur personnalisée
            valueAxis.IsAutomaticMaxValue = false;
            valueAxis.MaxValue = 40;
            Console.WriteLine("After change - IsAutomaticMaxValue: " + valueAxis.IsAutomaticMaxValue);
            Console.WriteLine("After change - MaxValue: " + valueAxis.MaxValue);

            // Réactiver la valeur maximale automatique
            valueAxis.IsAutomaticMaxValue = true;
            Console.WriteLine("After re-enabling - IsAutomaticMaxValue: " + valueAxis.IsAutomaticMaxValue);
            Console.WriteLine("After re-enabling - MaxValue: " + valueAxis.MaxValue);

            // Enregistrez le classeur
            workbook.Save("AxisPropertyIsAutomaticMaxValueDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


