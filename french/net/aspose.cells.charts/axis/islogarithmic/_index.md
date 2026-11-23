---
title: "Axis.IsLogarithmic"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Axis. Indique si le type d'échelle de l'axe des valeurs est logarithmique ou non"
type: docs
url: /fr/net/aspose.cells.charts/axis/islogarithmic/
---
## Axis.IsLogarithmic property

Représente si le type d'échelle de l'axe des valeurs est logarithmique ou non.

```csharp
public bool IsLogarithmic { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsLogarithmicDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(100);
            worksheet.Cells["A4"].PutValue(1000);
            worksheet.Cells["B1"].PutValue(5);
            worksheet.Cells["B2"].PutValue(25);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(100);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Ajouter une série
            chart.NSeries.Add("A1:A4", true);
            chart.NSeries[0].Values = "B1:B4";

            // Configurer l'axe logarithmique
            chart.CategoryAxis.IsLogarithmic = true;
            chart.CategoryAxis.LogBase = 10;
            chart.CategoryAxis.MinValue = 1;
            chart.CategoryAxis.MaxValue = 10000;

            // Enregistrez le classeur
            workbook.Save("AxisPropertyIsLogarithmicDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


