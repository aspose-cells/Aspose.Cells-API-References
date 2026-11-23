---
title: "ChartArea.Width"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartArea. Obtient ou définit le décalage horizontal de la colonne de son coin inférieur droit en unités de 1/4000 de la zone du graphique"
type: docs
url: /fr/net/aspose.cells.charts/chartarea/width/
---
## ChartArea.Width property

Obtient ou définit le décalage horizontal de la colonne de son coin inférieur droit, en unités de 1/4000 de la zone du graphique.

```csharp
[Obsolete("Use ChartArea.WidthRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Width { get; set; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. Veuillez utiliser la propriété ChartArea.WidthRatioToChart à la place. Width = WidthRatioToChart * 4000. Cette propriété sera supprimée 12 mois plus tard à compter de février 2025. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartAreaPropertyWidthDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtenez la zone du graphique
            ChartArea chartArea = chart.ChartArea;

            // Définir et démontrer la propriété Width
            Console.WriteLine("Original Width: " + chartArea.Width);
            chartArea.Width = 800; // Set new width
            Console.WriteLine("Modified Width: " + chartArea.Width);

            // Enregistrez le classeur
            workbook.Save("ChartAreaWidthDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


