---
title: "ChartGlobalizationSettings.GetAxisTitleName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartGlobalizationSettings metod. Hämtar namnet på titeln för axeln"
type: docs
url: /sv/net/aspose.cells.charts/chartglobalizationsettings/getaxistitlename/
---
## ChartGlobalizationSettings.GetAxisTitleName method

Hämtar namnet på Title för Axis.

```csharp
public virtual string GetAxisTitleName()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetAxisTitleNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Skapa globaliseringsinställningar och hämta axelns titelnamn
            ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();
            string axisTitleName = globalizationSettings.GetAxisTitleName();

            // Ange axelns titel
            chart.ValueAxis.Title.Text = axisTitleName;
            chart.CategoryAxis.Title.Text = axisTitleName;

            // Skriv ut axelns titelnamn
            Console.WriteLine("Axis Title Name: " + axisTitleName);

            // Spara arbetsboken
            workbook.Save("ChartGlobalizationSettingsDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


