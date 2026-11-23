---
title: "Axis.DisplayUnit"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Axis. Représente l'étiquette d'unité pour l'axe spécifié"
type: docs
url: /fr/net/aspose.cells.charts/axis/displayunit/
---
## Axis.DisplayUnit property

Représente l'étiquette d'unité pour l'axe spécifié.

```csharp
public DisplayUnitType DisplayUnit { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyDisplayUnitDemo
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
            worksheet.Cells["B2"].PutValue(10000);
            worksheet.Cells["B3"].PutValue(20000);
            worksheet.Cells["B4"].PutValue(30000);

            // Ajouter un graphique en colonnes
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Définir l'unité d'affichage de l'axe des valeurs en milliers
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Thousands;

            // Enregistrez le classeur
            workbook.Save("AxisPropertyDisplayUnitDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* enum [DisplayUnitType](../../displayunittype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


