---
title: "TickLabels.AutoScaleFont"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TickLabels. Vrai si le texte dans l'objet change de taille de police lorsque la taille de l'objet change. La valeur par défaut est Vrai"
type: docs
url: /fr/net/aspose.cells.charts/ticklabels/autoscalefont/
---
## TickLabels.AutoScaleFont property

Vrai si le texte de l'objet change de taille de police lorsque la taille de l'objet change. La valeur par défaut est Vrai.

```csharp
public bool AutoScaleFont { get; set; }
```

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyAutoScaleFontDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Données d'exemple
            cells["A1"].PutValue("Region");
            cells["A2"].PutValue("France");
            cells["A3"].PutValue("Germany");
            cells["A4"].PutValue("England");
            cells["B1"].PutValue("Sales");
            cells["B2"].PutValue(100000);
            cells["B3"].PutValue(150000);
            cells["B4"].PutValue(90000);

            // Créer un graphique
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 1, 20, 10);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Configurer les données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Configurer les étiquettes d'axe avec AutoScaleFont
            chart.CategoryAxis.TickLabels.AutoScaleFont = true;
            chart.CategoryAxis.TickLabels.Font.Size = 12; // Initial size
            
            // Enregistrez le classeur
            workbook.Save("TickLabelsAutoScaleFontDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


