---
title: "Axis.CustomUnit"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Axis-egenskap. Anger ett anpassat värde för visningsenheten"
type: docs
url: /sv/net/aspose.cells.charts/axis/customunit/
---
## Axis.CustomUnit property

Anger ett anpassat värde för visningsenheten.

```csharp
[Obsolete("Use Axis.CustomDisplayUnit property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int CustomUnit { get; set; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen Axis.CustomDisplayUnit. Denna egenskap kommer att tas bort 12 månader senare, från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisPropertyCustomUnitDemo
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
            worksheet.Cells["B2"].PutValue(1000000);
            worksheet.Cells["B3"].PutValue(2000000);
            worksheet.Cells["B4"].PutValue(3000000);

            // Lägg till ett stapeldiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Åtkomst till värdeaxeln
                Axis valueAxis = chart.ValueAxis;

                // Ställ in visningsenhet till anpassad
                valueAxis.DisplayUnit = DisplayUnitType.Custom;

                // Ställ in värde för anpassad visningsenhet
                valueAxis.CustomDisplayUnit = 1000000;

                // Visa värdet för egenskapen CustomUnit (föråldrad egenskap)
                Console.WriteLine("CustomUnit value: " + valueAxis.CustomUnit);

                // Spara arbetsboken
                workbook.Save("AxisPropertyCustomUnitDemo.xlsx");
                Console.WriteLine("CustomUnit has been demonstrated");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


