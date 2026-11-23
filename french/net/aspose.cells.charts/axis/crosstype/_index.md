---
title: "Axis.CrossType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Axis. Représente le CrossType sur l'axe spécifié où l'autre axe le croise"
type: docs
url: /fr/net/aspose.cells.charts/axis/crosstype/
---
## Axis.CrossType property

Représente le `CrossType` sur l'axe spécifié où l'autre axe le croise.

```csharp
public CrossType CrossType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyCrossTypeDemo
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

            // Créer un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Configurer l'axe des valeurs
            chart.ValueAxis.MaxValue = 200;
            chart.ValueAxis.MinValue = 0;
            chart.ValueAxis.MajorUnit = 25;
            
            // Démontrer la propriété CrossType
            chart.ValueAxis.CrossType = CrossType.Maximum;

            workbook.Save("AxisPropertyCrossTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [CrossType](../../crosstype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


