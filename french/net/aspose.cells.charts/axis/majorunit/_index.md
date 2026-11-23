---
title: "Axis.MajorUnit"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Axis. Représente les unités majeures de l'axe"
type: docs
url: /fr/net/aspose.cells.charts/axis/majorunit/
---
## Axis.MajorUnit property

Représente les unités majeures pour l'axe.

```csharp
public double MajorUnit { get; set; }
```

### Remarques

Les unités majeures doivent être supérieures à zéro.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMajorUnitDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Cat " + i);
                worksheet.Cells["B" + (i + 1)].PutValue(i * 10);
            }

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B11", true);
            chart.NSeries.CategoryData = "A2:A11";

            // Obtenir l'axe des catégories
            Axis axis = chart.CategoryAxis;

            // Afficher l'unité majeure initiale
            Console.WriteLine("Initial Major Unit: " + axis.MajorUnit);

            // Définir une nouvelle unité majeure
            axis.MajorUnit = 3;
            Console.WriteLine("Modified Major Unit: " + axis.MajorUnit);

            // Enregistrez le classeur
            workbook.Save("AxisMajorUnitDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


