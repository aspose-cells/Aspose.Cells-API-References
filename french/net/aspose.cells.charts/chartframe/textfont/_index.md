---
title: "ChartFrame.TextFont"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartFrame. Obtient un objet Font de l'objet ChartFrame spécifié"
type: docs
url: /fr/net/aspose.cells.charts/chartframe/textfont/
---
## ChartFrame.TextFont property

Obtient un objet [`Font`](../font/) de l'objet ChartFrame spécifié.

```csharp
[Obsolete("Use ChartFrame.Font property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual Font TextFont { get; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété ChartFrame.Font. Cette propriété sera supprimée 12 mois plus tard, depuis JANVIER 2012. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyTextFontDemo
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

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Définir le titre du graphique et configurer la police
            chart.Title.Text = "Sample Chart";
            chart.Title.TextFont.Name = "Arial";
            chart.Title.TextFont.Size = 14;
            chart.Title.TextFont.IsBold = true;
            chart.Title.TextFont.Color = System.Drawing.Color.Blue;

            // Enregistrez le classeur
            workbook.Save("ChartTitleFontDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Font](../../../aspose.cells/font/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


