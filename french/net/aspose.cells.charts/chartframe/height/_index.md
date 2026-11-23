---
title: "ChartFrame.Height"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartFrame. Obtient ou définit la hauteur du cadre en unités de 1/4000 de la zone du graphique"
type: docs
url: /fr/net/aspose.cells.charts/chartframe/height/
---
## ChartFrame.Height property

Obtient ou définit la hauteur du cadre en unités de 1/4000 de la zone du graphique.

```csharp
[Obsolete("Use ChartFrame.HeightRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int Height { get; set; }
```

### Remarques

Comment convertir les unités de 1/4000 en pixels ? Height In Pixels = Y * Chart.ChartObject.Height / 4000d;

NOTE : Ce membre est maintenant obsolète. Veuillez utiliser la propriété ChartFrame.HeightRatioToChart à la place. Height = HeightRatioToChart * 4000. Cette propriété sera supprimée 12 mois plus tard, à compter de février 2025. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyHeightDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accéder aux étiquettes de données
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            
            // Définir la propriété Height
            dataLabels.Height = 200; // Set height to 200 pixels
            
            // Afficher la valeur de la hauteur
            Console.WriteLine("DataLabels Height: " + dataLabels.Height);
            
            // Enregistrez le classeur
            workbook.Save("ChartFramePropertyHeightDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


