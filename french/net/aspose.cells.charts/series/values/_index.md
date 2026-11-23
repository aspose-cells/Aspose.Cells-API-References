---
title: "Series.Values"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Series. Représente les valeurs Y de cette série de graphique"
type: docs
url: /fr/net/aspose.cells.charts/series/values/
---
## Series.Values property

Représente les valeurs Y de cette série de graphique.

```csharp
public string Values { get; set; }
```

### Remarques

Pour obtenir les valeurs réelles (correspondant à chaque point de cette série) définies par cette propriété, veuillez utiliser [`PointValues`](../pointvalues/).

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyValuesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["C1"].PutValue("Series2");
            
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            worksheet.Cells["C2"].PutValue(15);
            worksheet.Cells["C3"].PutValue(25);
            worksheet.Cells["C4"].PutValue(35);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ajouter une série en utilisant la propriété Values
            chart.NSeries.Add("=Sheet1!$B$2:$B$4", true);
            chart.NSeries.Add("=Sheet1!$C$2:$C$4", true);

            // Définir les données de catégorie
            chart.NSeries.CategoryData = "=Sheet1!$A$2:$A$4";

            // Afficher la propriété Values pour chaque série
            Console.WriteLine("Series 1 Values: " + chart.NSeries[0].Values);
            Console.WriteLine("Series 2 Values: " + chart.NSeries[1].Values);

            // Enregistrez le classeur
            workbook.Save("SeriesPropertyValuesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


