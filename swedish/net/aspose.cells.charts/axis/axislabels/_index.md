---
title: "Axis.AxisLabels"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Axis property. Hämtar axelns etiketter efter anrop av metoden Chart.Calculate"
type: docs
url: /sv/net/aspose.cells.charts/axis/axislabels/
---
## Axis.AxisLabels property

Hämtar axelns etiketter efter anrop av metoden Chart.Calculate().

```csharp
[Obsolete("Use Axis.GetAxisTexts method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList AxisLabels { get; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället Axis.GetAxisTexts-metoden. Denna egenskap kommer att tas bort 12 månader senare från och med november 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisPropertyAxisLabelsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            try
            {
                // Lägg till ett diagram i kalkylbladet
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
                Chart chart = worksheet.Charts[chartIndex];

                // Ange diagrammets dataområde
                chart.NSeries.Add("B2:B4", true);
                chart.NSeries.CategoryData = "A2:A4";

                // Beräkna diagrammet för att generera axelns etiketter
                chart.Calculate();

                // Få åtkomst till kategoriaxeln och hämta axelns etiketter
                Axis categoryAxis = chart.CategoryAxis;
                var axisLabels = categoryAxis.AxisLabels;

                // Visa axelns etiketter
                Console.WriteLine("Axis Labels:");
                if (axisLabels != null)
                {
                    foreach (var label in axisLabels)
                    {
                        Console.WriteLine(label);
                    }
                }
                else
                {
                    Console.WriteLine("No axis labels available.");
                }

                // Spara arbetsboken
                workbook.Save("AxisPropertyAxisLabelsDemo.xlsx");
                Console.WriteLine("AxisLabels demonstration completed successfully.");
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


