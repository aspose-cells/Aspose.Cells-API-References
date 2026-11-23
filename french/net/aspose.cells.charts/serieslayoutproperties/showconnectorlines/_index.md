---
title: "SeriesLayoutProperties.ShowConnectorLines"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SeriesLayoutProperties. Indique si les lignes de connexion sont affichées entre les points de données"
type: docs
url: /fr/net/aspose.cells.charts/serieslayoutproperties/showconnectorlines/
---
## SeriesLayoutProperties.ShowConnectorLines property

Indique si les lignes de connexion sont affichées entre les points de données.

```csharp
public bool ShowConnectorLines { get; set; }
```

### Remarques

Uniquement pour le diagramme Waterfall.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyShowConnectorLinesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);

            // Ajouter un graphique
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            int seriesIndex = chart.NSeries.Add("A1:B4", true);
            Aspose.Cells.Charts.Series series = chart.NSeries[seriesIndex];

            // Définir ShowConnectorLines et d'autres propriétés
            Aspose.Cells.Charts.SeriesLayoutProperties layoutProperties = series.LayoutProperties;
            layoutProperties.ShowConnectorLines = true;
            layoutProperties.ShowMeanLine = true;

            workbook.Save("SeriesLayoutPropertiesShowConnectorLinesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


