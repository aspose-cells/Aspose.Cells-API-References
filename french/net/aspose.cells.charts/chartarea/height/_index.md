---
title: "ChartArea.Height"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartArea. Obtient ou définit le décalage vertical de la ligne de son coin inférieur droit en unités de 1/4000 de la zone du graphique"
type: docs
url: /fr/net/aspose.cells.charts/chartarea/height/
---
## ChartArea.Height property

Obtient ou définit le décalage vertical de la ligne de son coin inférieur‑droit, en unités de 1/4000 de la zone du graphique.

```csharp
[Obsolete("Use ChartArea.HeightRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Height { get; set; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. Veuillez utiliser la propriété ChartArea.HeightRatioToChart à la place. Height = HeightRatioToChart * 4000. Cette propriété sera supprimée 12 mois plus tard à compter de février 2025. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartAreaPropertyHeightDemo
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

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accéder à la zone du graphique
            ChartArea chartArea = chart.ChartArea;

            // Démontrer la propriété Height
            Console.WriteLine("Original Chart Area Height: " + chartArea.Height);
            
            // Modifier la hauteur
            chartArea.Height = 500;
            Console.WriteLine("Modified Chart Area Height: " + chartArea.Height);

            // Enregistrez le classeur
            workbook.Save("ChartAreaHeightDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


