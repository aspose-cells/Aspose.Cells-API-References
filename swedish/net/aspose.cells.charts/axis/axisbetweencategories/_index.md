---
title: "Axis.AxisBetweenCategories"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Axis-egenskap. Representerar om värdeaxeln korsar kategoriaxeln mellan kategorier"
type: docs
url: /sv/net/aspose.cells.charts/axis/axisbetweencategories/
---
## Axis.AxisBetweenCategories property

Representerar om värdeaxeln korsar kategoriaxeln mellan kategorier.

```csharp
public bool AxisBetweenCategories { get; set; }
```

### Anmärkningar

Denna egenskap gäller endast för kategoriaxlar och den gäller inte för 3‑D-diagram.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AxisPropertyAxisBetweenCategoriesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första kalkylbladet och lägg till exempeldata
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Categories");
            worksheet.Cells["B1"].PutValue("Values");
            
            for (int i = 1; i <= 5; i++)
            {
                worksheet.Cells[$"A{i+1}"].PutValue($"Category {i}");
                worksheet.Cells[$"B{i+1}"].PutValue(i * 10);
            }

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagramdata
            chart.NSeries.Add("B2:B6", true);
            chart.NSeries.CategoryData = "A2:A6";

            // Konfigurera kategoriaxeln
            Axis categoryAxis = chart.CategoryAxis;
            categoryAxis.AxisBetweenCategories = false; // Core property demonstration
            categoryAxis.TickLabels.RotationAngle = 45;

            // Spara arbetsboken
            workbook.Save("AxisBetweenCategoriesDemo.xlsx");
        }
    }
}
```

### Se även

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


