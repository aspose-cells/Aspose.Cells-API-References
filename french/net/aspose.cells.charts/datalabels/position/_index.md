---
title: "DataLabels.Position"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "DataLabels propriété. Représente la position de l'étiquette de données"
type: docs
url: /fr/net/aspose.cells.charts/datalabels/position/
---
## DataLabels.Position property

Représente la position de l'étiquette de données.

```csharp
public LabelPositionType Position { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyPositionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
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
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Activer les étiquettes de données
            chart.NSeries[0].DataLabels.ShowValue = true;
            
            // Définissez la position de l'étiquette de données
            chart.NSeries[0].DataLabels.Position = LabelPositionType.Right;

            // Enregistrez le classeur
            workbook.Save("DataLabelsPositionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [LabelPositionType](../../labelpositiontype/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


