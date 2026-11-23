---
title: "Chart.RightAngleAxes"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété du graphique. Vrai si les axes du graphique sont à angle droit. S'applique uniquement aux graphiques 3D sauf Column3D et graphiques 3D en secteurs"
type: docs
url: /fr/net/aspose.cells.charts/chart/rightangleaxes/
---
## Chart.RightAngleAxes property

Vrai si les axes du graphique sont perpendiculaires. S'applique uniquement aux graphiques 3D (sauf Column3D et graphiques 3D en secteurs).

```csharp
public bool RightAngleAxes { get; set; }
```

### Remarques

Si cette propriété est vraie, la propriété Perspective est ignorée.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyRightAngleAxesDemo
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
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // Ajouter un graphique à colonnes 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Démontrer la propriété RightAngleAxes
            chart.RightAngleAxes = true;
            Console.WriteLine("RightAngleAxes is set to: " + chart.RightAngleAxes);

            // Enregistrez le classeur
            workbook.Save("RightAngleAxesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


