---
title: "Line.Weight"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Line. Obtient ou définit le WeightType de la ligne"
type: docs
url: /fr/net/aspose.cells.drawing/line/weight/
---
## Line.Weight property

Obtient ou définit le [`WeightType`](../../weighttype/) de la ligne.

```csharp
public WeightType Weight { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyWeightDemo
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
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accéder à la zone du graphique et définir le poids de la bordure
            ChartArea chartArea = chart.ChartArea;
            chartArea.Border.Weight = WeightType.MediumLine;

            // Enregistrez le classeur
            workbook.Save("LinePropertyWeightDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* enum [WeightType](../../weighttype/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


