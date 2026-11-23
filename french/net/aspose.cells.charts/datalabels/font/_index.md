---
title: "DataLabels.Font"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataLabels. Obtient la police des DataLabels"
type: docs
url: /fr/net/aspose.cells.charts/datalabels/font/
---
## DataLabels.Font property

Obtient la police des DataLabels ;

```csharp
public override Font Font { get; }
```

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyFontDemo
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
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Activer les étiquettes de données
            Aspose.Cells.Charts.DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;

            // Définir les propriétés de la police
            dataLabels.Font.Color = Color.Red;
            dataLabels.Font.Size = 14;
            dataLabels.Font.IsBold = true;
            dataLabels.Font.Name = "Arial";

            // Enregistrez le classeur
            workbook.Save("DataLabelsFontDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [Font](../../../aspose.cells/font/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


