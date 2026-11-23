---
title: "Area.BackgroundColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Area. Obtient ou définit la couleur d'arrière-plan de l'Area"
type: docs
url: /fr/net/aspose.cells.drawing/area/backgroundcolor/
---
## Area.BackgroundColor property

Obtient ou définit la couleur d'arrière-plan de la [`Area`](../).

```csharp
public Color BackgroundColor { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class AreaPropertyBackgroundColorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
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
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Définissez la couleur d'arrière-plan pour la zone de l'axe des catégories
            chart.CategoryAxis.Area.BackgroundColor = System.Drawing.Color.Red;

            // Affichez la couleur d'arrière-plan
            Console.WriteLine("Category Axis Background Color: " + chart.CategoryAxis.Area.BackgroundColor);

            // Enregistrez le classeur
            workbook.Save("AreaPropertyBackgroundColorDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


