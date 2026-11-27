---
title: "Axis.MinorUnit"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Axis-egenskap. Representerar de mindre enheterna för axeln"
type: docs
url: /sv/net/aspose.cells.charts/axis/minorunit/
---
## Axis.MinorUnit property

Anger sekundära enheter för axeln.

```csharp
public double MinorUnit { get; set; }
```

### Anmärkningar

De mindre enheterna måste vara större än noll.

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMinorUnitDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Lägg till exempeldata
            cells["A1"].PutValue("Region");
            cells["A2"].PutValue("France");
            cells["A3"].PutValue("Germany");
            cells["A4"].PutValue("England");
            cells["B1"].PutValue("Sales");
            cells["B2"].PutValue(70000);
            cells["B3"].PutValue(55000);
            cells["B4"].PutValue(30000);

            // Skapa diagram
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 1, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Konfigurera diagramdata
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Konfigurera värdeaxeln
            chart.ValueAxis.Title.Text = "Sales Amount";
            chart.ValueAxis.MajorUnit = 20000;
            chart.ValueAxis.MinorUnit = 5000; // Demonstrate MinorUnit property
            chart.ValueAxis.MinValue = 0;
            chart.ValueAxis.MaxValue = 80000;

            // Spara arbetsboken
            workbook.Save("AxisPropertyMinorUnitDemo.xlsx");
        }
    }
}
```

### Se även

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


