---
title: "ChartFrame.Font"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartFrame. Obtient un objet Font de l'objet ChartFrame spécifié"
type: docs
url: /fr/net/aspose.cells.charts/chartframe/font/
---
## ChartFrame.Font property

Obtient un objet `Font` de l'objet ChartFrame spécifié.

```csharp
public virtual Font Font { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyFontDemo
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Définir le titre du graphique et configurer les propriétés de la police
            chart.Title.Text = "Sample Chart";
            chart.Title.Font.Name = "Arial";
            chart.Title.Font.Size = 14;
            chart.Title.Font.Color = System.Drawing.Color.Blue;
            chart.Title.Font.CapsType = TextCapsType.None;
            chart.Title.Font.IsBold = true;

            // Enregistrez le classeur
            workbook.Save("ChartFontDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Font](../../../aspose.cells/font/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


