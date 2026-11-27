---
title: "ChartGlobalizationSettings.GetAxisUnitName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartGlobalizationSettings metod. Hämtar namnet på axelns enhet"
type: docs
url: /sv/net/aspose.cells.charts/chartglobalizationsettings/getaxisunitname/
---
## ChartGlobalizationSettings.GetAxisUnitName method

Hämtar namnet på Axis Unit.

```csharp
public virtual string GetAxisUnitName(DisplayUnitType type)
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetAxisUnitNameWithDisplayUnitTypeDemo
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
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);

            // Lägg till diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Skapa globaliseringsinställningar och hämta axelns enhetsnamn
            ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();
            string thousandsUnit = globalizationSettings.GetAxisUnitName(DisplayUnitType.Thousands);
            string millionsUnit = globalizationSettings.GetAxisUnitName(DisplayUnitType.Millions);

            // Skriv ut resultat
            Console.WriteLine("Thousands unit name: " + thousandsUnit);
            Console.WriteLine("Millions unit name: " + millionsUnit);

            // Spara arbetsbok
            workbook.Save("AxisUnitNameDemo.xlsx");
        }
    }
}
```

### Se även

* enum [DisplayUnitType](../../displayunittype/)
* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


