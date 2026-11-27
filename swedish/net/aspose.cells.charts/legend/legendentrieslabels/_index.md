---
title: "Legend.LegendEntriesLabels"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Legend-egenskap. Hämtar etiketterna för legendposterna efter att Chart.Calculate-metoden har anropats"
type: docs
url: /sv/net/aspose.cells.charts/legend/legendentrieslabels/
---
## Legend.LegendEntriesLabels property

Hämtar etiketterna för legendposterna efter att Chart.Calculate()-metoden har anropats.

```csharp
[Obsolete("Use Legend.GetLegendLabels method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList LegendEntriesLabels { get; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället Legend.GetLegendLabels-metoden. Denna egenskap kommer att tas bort 12 månader senare sedan november 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LegendPropertyLegendEntriesLabelsDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Beräkna diagrammet för att säkerställa att legendposterna genereras
            chart.Calculate();

            // Hämta legenden
            Legend legend = chart.Legend;

            // Visa legendposternas etiketter (med hjälp av egenskapen)
            Console.WriteLine("Legend Entries Labels:");
            foreach (string label in legend.LegendEntriesLabels)
            {
                Console.WriteLine(label);
            }

            // Spara arbetsboken
            workbook.Save("LegendEntriesLabelsDemo.xlsx");
        }
    }
}
```

### Se även

* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


