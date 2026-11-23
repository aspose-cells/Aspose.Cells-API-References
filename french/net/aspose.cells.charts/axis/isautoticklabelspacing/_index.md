---
title: "Axis.IsAutoTickLabelSpacing"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Axis. Indique si l'espacement des libellés de graduation est automatique"
type: docs
url: /fr/net/aspose.cells.charts/axis/isautoticklabelspacing/
---
## Axis.IsAutoTickLabelSpacing property

Indique si l'espacement des étiquettes de graduation est automatique

```csharp
public bool IsAutoTickLabelSpacing { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsAutoTickLabelSpacingDemo
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

            // Configurer l'axe des valeurs
            Axis valueAxis = chart.ValueAxis;
            valueAxis.IsAutoTickLabelSpacing = true; // Core property demonstration
            
            // Configurer l'axe des catégories
            Axis categoryAxis = chart.CategoryAxis;
            categoryAxis.IsAutoTickLabelSpacing = false; // Core property demonstration
            categoryAxis.TickLabelSpacing = 2;

            workbook.Save("AxisPropertyIsAutoTickLabelSpacingDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


