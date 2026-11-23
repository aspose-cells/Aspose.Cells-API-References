---
title: "ChartTextFrame.Text"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartTextFrame. Obtient ou définit le texte du titre d'un cadre"
type: docs
url: /fr/net/aspose.cells.charts/charttextframe/text/
---
## ChartTextFrame.Text property

Obtient ou définit le texte du titre d'un cadre.

```csharp
public virtual string Text { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyTextDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Category");
            cells["A2"].PutValue("A");
            cells["A3"].PutValue("B");
            cells["A4"].PutValue("C");
            cells["B1"].PutValue("Value");
            cells["B2"].PutValue(10);
            cells["B3"].PutValue(20);
            cells["B4"].PutValue(30);

            // Ajouter un graphique
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Définir le texte du titre du graphique
            chart.Title.Text = "Sample Chart Title";

            // Accéder et modifier le texte de la légende
            Legend legend = chart.Legend;
            legend.Text = "Custom Legend Text";

            // Enregistrez le classeur
            workbook.Save("ChartTextDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


