---
title: "Chart.Elevation"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Chart propriété. Représente l'élévation de la vue du graphique 3D en degrés"
type: docs
url: /fr/net/aspose.cells.charts/chart/elevation/
---
## Chart.Elevation property

Représente l'élévation de la vue du graphique 3D, en degrés.

```csharp
public int Elevation { get; set; }
```

### Remarques

L'élévation du graphique est la hauteur à laquelle vous visualisez le graphique, en degrés. La valeur par défaut est 15 pour la plupart des types de graphiques. La valeur de cette propriété doit être comprise entre -90 et 90, sauf pour les graphiques à barres 3-D, où elle doit être comprise entre 0 et 44.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyElevationDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Ajouter un graphique à colonnes 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Définir la propriété d'élévation (angle en degrés)
            chart.Elevation = 30;
            
            // Enregistrez le classeur
            workbook.Save("ChartElevationDemo.xlsx");

            Console.WriteLine("Chart created with elevation set to 30 degrees.");
        }
    }
}
```

### Voir aussi

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


