---
title: "Trendline.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Trendline. Renvoie le type de ligne de tendance"
type: docs
url: /fr/net/aspose.cells.charts/trendline/type/
---
## Trendline.Type property

Renvoie le type de courbe de tendance.

```csharp
public TrendlineType Type { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue("X");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["A4"].PutValue(3);
            sheet.Cells["A5"].PutValue(4);
            
            sheet.Cells["B1"].PutValue("Y");
            sheet.Cells["B2"].PutValue(2);
            sheet.Cells["B3"].PutValue(4);
            sheet.Cells["B4"].PutValue(8);
            sheet.Cells["B5"].PutValue(16);

            // Ajoutez un graphique
            int chartIndex = sheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Ajouter une série
            chart.NSeries.Add("A2:A5", true);
            chart.NSeries[0].XValues = "B2:B5";

            // Ajouter une ligne de tendance exponentielle
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Exponential);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            
            // Démontrer l'utilisation de la propriété Type
            Console.WriteLine("Trendline type: " + trendline.Type);
            
            // Enregistrez le classeur
            workbook.Save("TrendlinePropertyTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [TrendlineType](../../trendlinetype/)
* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


