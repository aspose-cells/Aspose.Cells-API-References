---
title: "ChartGlobalizationSettings.GetOtherName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartGlobalizationSettings-metod. Hämtar namnet på Other-etiketter för diagrammet"
type: docs
url: /sv/net/aspose.cells.charts/chartglobalizationsettings/getothername/
---
## ChartGlobalizationSettings.GetOtherName method

Hämtar namnet på "Other"-etiketter för Chart.

```csharp
public virtual string GetOtherName()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetOtherNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Lägg till diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Skapa globaliseringsinställningar och hämta annat namn
            ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();
            string otherName = globalizationSettings.GetOtherName();

            // Skriv ut resultatet
            Console.WriteLine("Other Name: " + otherName);

            // Spara arbetsbok
            workbook.Save("ChartGlobalizationDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


