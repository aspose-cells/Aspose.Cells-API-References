---
title: "Line.DashType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Line. Spécifie le type de ligne en pointillés"
type: docs
url: /fr/net/aspose.cells.drawing/line/dashtype/
---
## Line.DashType property

Spécifie le type de ligne en pointillé

```csharp
public MsoLineDashStyle DashType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyDashTypeDemo
    {
        public static void Run()
        {
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

            // Créer un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Personnaliser le type de tiret de la ligne de série
            chart.CategoryAxis.MajorGridLines.DashType = MsoLineDashStyle.DashDot;
            chart.CategoryAxis.MinorGridLines.DashType = MsoLineDashStyle.DashLongDashDot;

            // Personnaliser la ligne de série
            chart.NSeries[0].Border.DashType = MsoLineDashStyle.Solid;
            chart.NSeries[0].Border.Color = System.Drawing.Color.Blue;

            workbook.Save("LineDashTypeDemo.xlsx");
            Console.WriteLine("Line chart with custom dash types created successfully.");
        }
    }
}
```

### Voir aussi

* enum [MsoLineDashStyle](../../msolinedashstyle/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


