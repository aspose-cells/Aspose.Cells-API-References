---
title: "Axis.MaxValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Axis. Représente la valeur maximale sur l'axe des valeurs"
type: docs
url: /fr/net/aspose.cells.charts/axis/maxvalue/
---
## Axis.MaxValue property

Représente la valeur maximale sur l'axe des valeurs.

```csharp
public object MaxValue { get; set; }
```

### Remarques

Le type maxValue ne peut être que double ou DateTime

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMaxValueDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(50);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Définir la valeur maximale de l'axe des valeurs
            chart.ValueAxis.MaxValue = 60;

            // Enregistrez le classeur
            workbook.Save("AxisPropertyMaxValueDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


