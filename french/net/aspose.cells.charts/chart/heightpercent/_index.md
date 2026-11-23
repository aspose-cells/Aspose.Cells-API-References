---
title: "Chart.HeightPercent"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Chart propriété. Retourne ou définit la hauteur d'un graphique 3D en pourcentage de la largeur du graphique, entre 5 et 500 pour cent"
type: docs
url: /fr/net/aspose.cells.charts/chart/heightpercent/
---
## Chart.HeightPercent property

Renvoie ou définit la hauteur d'un graphique 3D en pourcentage de la largeur du graphique (entre 5 et 500 pour cent).

```csharp
public int HeightPercent { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyHeightPercentDemo
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

            // Ajouter un graphique à colonnes 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Définir la propriété HeightPercent (contrôle la hauteur du graphique 3D en pourcentage de la largeur du graphique)
            chart.HeightPercent = 150; // 150% of chart width

            // Enregistrez le classeur
            workbook.Save("ChartHeightPercentDemo.xlsx");

            Console.WriteLine("Chart with HeightPercent 150% created successfully.");
        }
    }
}
```

### Voir aussi

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


