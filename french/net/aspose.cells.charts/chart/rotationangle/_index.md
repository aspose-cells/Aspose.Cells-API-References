---
title: "Chart.RotationAngle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Chart propriété. Représente la rotation de la vue du graphique 3D, la rotation de la zone de tracé autour de l'axe z en degrés"
type: docs
url: /fr/net/aspose.cells.charts/chart/rotationangle/
---
## Chart.RotationAngle property

Représente la rotation de la vue du graphique 3D (la rotation de la zone du tracé autour de l'axe z, en degrés).

```csharp
public int RotationAngle { get; set; }
```

### Remarques

La valeur de cette propriété doit être comprise entre 0 et 360, sauf pour les graphiques à barres 3D, où la valeur doit être comprise entre 0 et 44. La valeur par défaut est 20. S'applique uniquement aux graphiques 3D.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyRotationAngleDemo
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

            // Définissez l'angle de rotation à 45 degrés
            chart.RotationAngle = 45;

            // Enregistrez le classeur
            workbook.Save("ChartRotationAngleDemo.xlsx");

            Console.WriteLine("Chart with rotation angle created successfully.");
        }
    }
}
```

### Voir aussi

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


