---
title: "SeriesLayoutProperties.ShowMeanLine"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SeriesLayoutProperties. Indique s'il faut afficher la ligne reliant tous les points moyens"
type: docs
url: /fr/net/aspose.cells.charts/serieslayoutproperties/showmeanline/
---
## SeriesLayoutProperties.ShowMeanLine property

Indique si la ligne reliant tous les points moyens doit être affichée.

```csharp
public bool ShowMeanLine { get; set; }
```

### Remarques

Fonctionne uniquement pour le graphique BoxWhisker.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyShowMeanLineDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le diagramme à moustaches
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(40);
            worksheet.Cells["A4"].PutValue(25);
            worksheet.Cells["A5"].PutValue(40);
            worksheet.Cells["A6"].PutValue(115);
            worksheet.Cells["A7"].PutValue(65.666);

            // Ajouter un diagramme à moustaches
            int chartIndex = worksheet.Charts.Add(ChartType.BoxWhisker, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ajouter des séries au graphique
            chart.NSeries.Add("A1:A7", true);

            // Obtenir la première série
            Series series = chart.NSeries[0];

            // Accéder aux propriétés de mise en page
            SeriesLayoutProperties layout = series.LayoutProperties;

            // Démontrer la propriété ShowMeanLine
            Console.WriteLine("Default ShowMeanLine value: " + layout.ShowMeanLine);
            
            // Définir ShowMeanLine sur true
            layout.ShowMeanLine = true;
            Console.WriteLine("After setting ShowMeanLine to true: " + layout.ShowMeanLine);

            // Enregistrez le classeur
            workbook.Save("BoxWhiskerChart_ShowMeanLineDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


