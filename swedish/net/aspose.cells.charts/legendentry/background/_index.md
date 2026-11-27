---
title: "LegendEntry.Background"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LegendEntry egenskap. Hämtar och anger visningsläget för bakgrunden"
type: docs
url: /sv/net/aspose.cells.charts/legendentry/background/
---
## LegendEntry.Background property

Hämtar och anger visningsläget för bakgrunden

```csharp
[Obsolete("Use LegendEntry.BackgroundMode property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public BackgroundMode Background { get; set; }
```

### Anmärkningar

OBS: Den här medlemmen är nu föråldrad. Använd istället egenskapen LegendEntry.BackgroundMode. Denna egenskap kommer att tas bort 12 månader senare sedan JANUARY 2012. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LegendEntryPropertyBackgroundDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Hämta den första legendposten
                LegendEntry legendEntry = chart.Legend.LegendEntries[0];

                // Visa det aktuella värdet för egenskapen Background
                Console.WriteLine("Current Background value: " + legendEntry.Background);

                // Ange ett nytt Background‑värde (eftersom det inte är skrivskyddat)
                legendEntry.Background = BackgroundMode.Opaque;
                Console.WriteLine("Background after setting to Opaque: " + legendEntry.Background);

                // Ange ett annat Background‑värde
                legendEntry.Background = BackgroundMode.Transparent;
                Console.WriteLine("Background after setting to Transparent: " + legendEntry.Background);

                // Spara arbetsboken
                workbook.Save("LegendEntryBackgroundDemo.xlsx");
                Console.WriteLine("Background property demonstration completed successfully.");
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

* enum [BackgroundMode](../../backgroundmode/)
* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


