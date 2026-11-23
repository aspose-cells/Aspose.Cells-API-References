---
title: "Series.IsVerticalValues"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Series. Indique si la source de données est verticale"
type: docs
url: /fr/net/aspose.cells.charts/series/isverticalvalues/
---
## Series.IsVerticalValues property

Indique si la source de données est verticale.

```csharp
public bool IsVerticalValues { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyIsVerticalValuesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue("Cat " + (i-1));
                worksheet.Cells["B" + i].PutValue(i * 10);
            }

            // Ajouter un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ajouter une série avec des valeurs verticales
            chart.NSeries.Add("A1:B10", true);
            
            // Démontrer la propriété IsVerticalValues (lecture seule)
            Console.WriteLine("IsVerticalValues for first series: " + chart.NSeries[0].IsVerticalValues);
            
            // Pour changer l'orientation, nous devons recréer la série avec des paramètres différents
            chart.NSeries.Clear();
            chart.NSeries.Add("A1:B10", false);
            Console.WriteLine("IsVerticalValues after recreation: " + chart.NSeries[0].IsVerticalValues);
        }
    }
}
```

### Voir aussi

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


