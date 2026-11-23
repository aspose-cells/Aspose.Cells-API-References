---
title: "Series.CountOfDataValues"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Series. Obtient le nombre de valeurs de données"
type: docs
url: /fr/net/aspose.cells.charts/series/countofdatavalues/
---
## Series.CountOfDataValues property

Obtient le nombre de valeurs de données.

```csharp
public int CountOfDataValues { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyCountOfDataValuesDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple aux cellules
            for (int i = 0; i < 4; i++)
            {
                worksheet.Cells[i, 0].PutValue(i + 1); // A1:A4 with values 1-4
            }

            // Créer un graphique
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ajouter une série en utilisant la plage de données
            chart.NSeries.Add("A1:A4", true);
            
            // Afficher le nombre de valeurs de données dans la première série
            Console.WriteLine("Count of data values in series: " + chart.NSeries[0].CountOfDataValues);
            
            // Enregistrez le classeur
            workbook.Save("SeriesPropertyCountOfDataValuesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


