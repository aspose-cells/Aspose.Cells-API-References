---
title: "Line.Style"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Line. Représente le style de la ligne"
type: docs
url: /fr/net/aspose.cells.drawing/line/style/
---
## Line.Style property

Représente le style de la ligne.

```csharp
public LineType Style { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer un graphique d'exemple
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // Obtenir la première série et son premier point
            Series series = chart.NSeries[0];
            ChartPoint point = series.Points[0];
            
            // Définir les propriétés de la ligne
            point.Border.Color = Color.Red;
            point.Border.Style = LineType.Solid;
            
            // Vérifier que le style a été défini
            Console.WriteLine("Border Style: " + point.Border.Style);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* enum [LineType](../../linetype/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


