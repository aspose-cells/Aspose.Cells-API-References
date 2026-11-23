---
title: "Series.Has3DEffect"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété de Series. Vrai si la série a un aspect tridimensionnel"
type: docs
url: /fr/net/aspose.cells.charts/series/has3deffect/
---
## Series.Has3DEffect property

Vrai si la série a un aspect tridimensionnel.

```csharp
public bool Has3DEffect { get; set; }
```

### Remarques

S'applique uniquement aux graphiques Bulles ou Bulles3D.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyHas3DEffectDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Q3");

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ajouter une série
            int seriesIndex = chart.NSeries.Add("A1:B3", true);
            chart.NSeries.CategoryData = "C1:C3";
            
            // Obtenir la série et définir l'effet 3D
            Series series = chart.NSeries[seriesIndex];
            series.Has3DEffect = true;
            series.Bar3DShapeType = Bar3DShapeType.Cylinder;

            // Enregistrez le classeur
            workbook.Save("Series3DEffectDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


