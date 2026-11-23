---
title: "Axis.TickMarkSpacing"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Axis. Retourne ou définit le nombre de catégories ou de séries entre les marques de graduation. S'applique uniquement aux axes de catégorie et de séries"
type: docs
url: /fr/net/aspose.cells.charts/axis/tickmarkspacing/
---
## Axis.TickMarkSpacing property

Renvoie ou définit le nombre de catégories ou de séries entre les repères. S'applique uniquement aux axes de catégorie et de séries.

```csharp
public int TickMarkSpacing { get; set; }
```

### Remarques

Le nombre doit être compris entre 1 et 31999.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyTickMarkSpacingDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Ajouter un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Configurer l'axe des valeurs avec TickMarkSpacing
            Axis valueAxis = chart.ValueAxis;
            valueAxis.MinValue = 0;
            valueAxis.MaxValue = 200;
            valueAxis.MajorUnit = 25;
            valueAxis.MinorUnit = 5;
            valueAxis.TickMarkSpacing = 2; // Setting tick mark spacing
            
            // Configurer l'axe de catégorie avec TickMarkSpacing
            Axis categoryAxis = chart.CategoryAxis;
            categoryAxis.TickMarkSpacing = 1; // Setting tick mark spacing

            workbook.Save("AxisTickMarkSpacingDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


