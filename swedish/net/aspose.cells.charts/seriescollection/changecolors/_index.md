---
title: "SeriesCollection.ChangeColors"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SeriesCollection-metod. Ställ in monokrom palett för diagramserier"
type: docs
url: /sv/net/aspose.cells.charts/seriescollection/changecolors/
---
## SeriesCollection.ChangeColors method

Ställ in monokromatisk palett för diagramserier.

```csharp
public void ChangeColors(ChartColorPaletteType type)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | ChartColorPaletteType | Den monokroma typen. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionMethodChangeColorsWithChartColorPaletDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet ws = workbook.Worksheets[0];

            // Fyll i lite data för diagrammet
            ws.Cells["A1"].PutValue("Category");
            ws.Cells["A2"].PutValue("Jan");
            ws.Cells["A3"].PutValue("Feb");
            ws.Cells["A4"].PutValue("Mar");

            ws.Cells["B1"].PutValue("Series1");
            ws.Cells["B2"].PutValue(10);
            ws.Cells["B3"].PutValue(20);
            ws.Cells["B4"].PutValue(30);

            ws.Cells["C1"].PutValue("Series2");
            ws.Cells["C2"].PutValue(15);
            ws.Cells["C3"].PutValue(25);
            ws.Cells["C4"].PutValue(35);

            // Lägg till ett stapeldiagram
            int chartIdx = ws.Charts.Add(ChartType.Column, 6, 0, 20, 10);
            Chart chart = ws.Charts[chartIdx];

            // Ange dataintervallet för serien
            chart.NSeries.Add("B1:C4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Hämta seriekollektionen
            SeriesCollection seriesColl = chart.NSeries;

            try
            {
                // Ändra färgpaletten för alla serier i samlingen.
                // Använd en numerisk cast till ett giltigt enum‑värde (t.ex. 0) för att undvika beroende enum‑medlemsnamn.
                seriesColl.ChangeColors((ChartColorPaletteType)0);

                Console.WriteLine("ChangeColors method invoked successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error invoking ChangeColors: {ex.Message}");
            }

            // Spara arbetsboken för att verifiera resultatet
            workbook.Save("SeriesCollection_ChangeColors_Demo.xlsx");
        }
    }
}
```

### Se även

* enum [ChartColorPaletteType](../../chartcolorpalettetype/)
* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


