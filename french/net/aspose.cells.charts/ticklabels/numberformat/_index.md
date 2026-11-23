---
title: "TickLabels.NumberFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TickLabels. Représente la chaîne de format pour l'objet TickLabels"
type: docs
url: /fr/net/aspose.cells.charts/ticklabels/numberformat/
---
## TickLabels.NumberFormat property

Représente la chaîne de format pour l'objet TickLabels.

```csharp
public string NumberFormat { get; set; }
```

### Remarques

La chaîne de format est identique à une chaîne de format personnalisée appliquée à une cellule. Par exemple, \"$0\".

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyNumberFormatDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(1.2345);
            worksheet.Cells["A3"].PutValue(2.3456);
            worksheet.Cells["A4"].PutValue(3.4567);

            // Créer un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.NSeries.Add("A2:A4", true);

            // Définir le format numérique pour les étiquettes de graduation de l'axe des valeurs
            chart.ValueAxis.TickLabels.NumberFormat = "0.00";

            // Enregistrez le classeur
            workbook.Save("TickLabelsNumberFormatDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


