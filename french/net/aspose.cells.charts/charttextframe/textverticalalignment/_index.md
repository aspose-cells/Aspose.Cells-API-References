---
title: "ChartTextFrame.TextVerticalAlignment"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartTextFrame. Obtient ou définit l'alignement vertical du texte"
type: docs
url: /fr/net/aspose.cells.charts/charttextframe/textverticalalignment/
---
## ChartTextFrame.TextVerticalAlignment property

Obtient ou définit l'alignement vertical du texte.

```csharp
public TextAlignmentType TextVerticalAlignment { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyTextVerticalAlignmentDemo
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

            // Ajouter un graphique en colonnes
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Définir le titre et configurer l'alignement vertical
            chart.Title.Text = "Sample Chart";
            chart.Title.TextVerticalAlignment = TextAlignmentType.Top;

            // Configurer l'étiquette d'unité d'affichage
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds;
            chart.ValueAxis.DisplayUnitLabel.Text = "Values in Hundreds";
            chart.ValueAxis.DisplayUnitLabel.TextVerticalAlignment = TextAlignmentType.Center;

            // Enregistrez le classeur
            workbook.Save("ChartTextVerticalAlignmentDemo.xlsx");

            Console.WriteLine("Demo executed successfully. Output file: ChartTextVerticalAlignmentDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


