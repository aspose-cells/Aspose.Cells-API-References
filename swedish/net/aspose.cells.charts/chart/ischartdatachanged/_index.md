---
title: "Chart.IsChartDataChanged"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart-metod. Upptäcker om diagrammets datakälla har ändrats"
type: docs
url: /sv/net/aspose.cells.charts/chart/ischartdatachanged/
---
## Chart.IsChartDataChanged method

Detekterar om diagrammets datakälla har ändrats.

```csharp
public bool IsChartDataChanged()
```

### Returvärde

Returnerar true om diagrammet har ändrats, annars returneras false

### Anmärkningar

Metoden upptäcker förändringarna i diagrammets datakälla innan diagrammet renderas till bildformat. Vid första anropet av `Chart.toImage` kommer diagrammets källdata (t.ex. XValuesParseData, ValuesParseData) att registreras. Innan du anropar `Chart.toImage`-metoden igen, anropa `IsChartDataChanged`-metoden för att kontrollera om diagrammet behöver renderas om.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartMethodIsChartDataChangedDemo
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

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataområde
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // Kontrollera om diagramdata har ändrats (bör vara false initialt)
                bool isChanged = chart.IsChartDataChanged();
                Console.WriteLine($"Chart data changed after creation: {isChanged}");

                // Modifiera diagramdata
                worksheet.Cells["B2"].PutValue(15);

                // Kontrollera igen om diagramdata har ändrats
                isChanged = chart.IsChartDataChanged();
                Console.WriteLine($"Chart data changed after modification: {isChanged}");

                // Beräkna diagrammet för att uppdatera det
                chart.Calculate();

                // Kontrollera efter beräkning
                isChanged = chart.IsChartDataChanged();
                Console.WriteLine($"Chart data changed after calculation: {isChanged}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsChartDataChanged method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("ChartMethodIsChartDataChangedDemo.xlsx");
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


