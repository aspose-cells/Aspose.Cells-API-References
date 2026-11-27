---
title: "Chart.ChangeTemplate"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Diagrammetod. Ändra diagramtyp med en förinställd mall"
type: docs
url: /sv/net/aspose.cells.charts/chart/changetemplate/
---
## Chart.ChangeTemplate method

Ändra diagramtyp med en förinställd mall.

```csharp
public void ChangeTemplate(byte[] data)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| data | Byte[] | Data för diagrammallfil (.crtx). |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.IO;

    public class ChartMethodChangeTemplateWithByteDemo
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
            chart.SetChartDataRange("A1:B4", false);

            // Hämta malldata från en annan diagramfil
            byte[] templateData = File.ReadAllBytes("ChartTemplate.crtx");

            try
            {
                // Anropa ChangeTemplate-metoden med byte-arrayparameter
                chart.ChangeTemplate(templateData);
                
                Console.WriteLine("Chart template changed successfully using byte array parameter");
                
                // Visa effekten genom att spara arbetsboken
                workbook.Save("ChartWithChangedTemplate.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error changing chart template: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


