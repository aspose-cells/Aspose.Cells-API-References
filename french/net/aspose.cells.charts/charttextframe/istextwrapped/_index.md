---
title: "ChartTextFrame.IsTextWrapped"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartTextFrame. Obtient ou définit une valeur indiquant si le texte est renvoyé à la ligne"
type: docs
url: /fr/net/aspose.cells.charts/charttextframe/istextwrapped/
---
## ChartTextFrame.IsTextWrapped property

Obtient ou définit une valeur indiquant si le texte est renvoyé à la ligne.

```csharp
public virtual bool IsTextWrapped { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyIsTextWrappedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Q1");
            sheet.Cells["A3"].PutValue("Q2");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(12000);
            sheet.Cells["B3"].PutValue(15000);

            // Ajouter un graphique
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 5, 20, 10);
            Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Définir le titre du graphique avec retour à la ligne du texte
            chart.Title.Text = "Quarterly Sales Report (2023) - This is a long title that will wrap when IsTextWrapped is true";
            chart.Title.IsTextWrapped = true;
            
            // Enregistrer le classeur
            workbook.Save("ChartTextWrappingDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


