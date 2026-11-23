---
title: "Legend.Position"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Legend. Obtient ou définit le type de position de la légende"
type: docs
url: /fr/net/aspose.cells.charts/legend/position/
---
## Legend.Position property

Obtient ou définit le type de position de la légende.

```csharp
public LegendPositionType Position { get; set; }
```

### Remarques

La position par défaut est à droite. Si la légende se trouve du côté gauche ou droit du graphique, la définition de la propriété Legend.X n'aura aucun effet. Si la légende se trouve du côté supérieur ou inférieur du graphique, la définition de la propriété Legend.Y n'aura aucun effet.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendPropertyPositionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Ajoutez un graphique
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Définir la position de la légende
            chart.Legend.Position = LegendPositionType.Left;

            // Enregistrez le classeur
            workbook.Save("LegendPositionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [LegendPositionType](../../legendpositiontype/)
* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


