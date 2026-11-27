---
title: "Axis.MajorUnit"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Axis-egenskap. Representerar huvud‑enheterna för axeln"
type: docs
url: /sv/net/aspose.cells.charts/axis/majorunit/
---
## Axis.MajorUnit property

Anger huvudenheterna för axeln.

```csharp
public double MajorUnit { get; set; }
```

### Anmärkningar

De stora enheterna måste vara större än noll.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMajorUnitDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Cat " + i);
                worksheet.Cells["B" + (i + 1)].PutValue(i * 10);
            }

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B11", true);
            chart.NSeries.CategoryData = "A2:A11";

            // Hämta kategoriekaxeln
            Axis axis = chart.CategoryAxis;

            // Visa den initiala huvudenheten
            Console.WriteLine("Initial Major Unit: " + axis.MajorUnit);

            // Ställ in ny huvudenhet
            axis.MajorUnit = 3;
            Console.WriteLine("Modified Major Unit: " + axis.MajorUnit);

            // Spara arbetsboken
            workbook.Save("AxisMajorUnitDemo.xlsx");
        }
    }
}
```

### Se även

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


