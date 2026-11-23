---
title: "ChartCollection.AddFloatingChart"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ChartCollection. Ajoute un graphique à la collection"
type: docs
url: /fr/net/aspose.cells.charts/chartcollection/addfloatingchart/
---
## ChartCollection.AddFloatingChart method

Ajoute un graphique à la collection.

```csharp
public int AddFloatingChart(ChartType type, int left, int top, int width, int height)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | ChartType | Type de graphique |
| gauche | Int32 | Le décalage x vers le coin |
| haut | Int32 | Le décalage y vers le coin |
| largeur | Int32 | La largeur du graphique |
| hauteur | Int32 | La hauteur du graphique |

### Valeur de retour

[`Chart`](../../chart/) object index.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCollectionMethodAddFloatingChartWithChartTypeInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajouter un graphique flottant avec les dimensions spécifiées
            int chartIndex = sheet.Charts.AddFloatingChart(ChartType.Column, 100, 100, 600, 400);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Ajouter des données d'exemple au graphique
            chart.NSeries.Add("{1,3,2,5}", false);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


