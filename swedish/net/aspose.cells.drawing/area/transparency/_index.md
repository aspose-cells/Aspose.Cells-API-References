---
title: "Area.Transparency"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Area-egenskap. Returnerar eller anger transparensgraden för området som ett värde från 0.0 ogenomskinligt till 1.0 helt genomskinligt"
type: docs
url: /sv/net/aspose.cells.drawing/area/transparency/
---
## Area.Transparency property

Returnerar eller anger graden av transparens för området som ett värde från 0,0 (opak) till 1,0 (klar).

```csharp
public double Transparency { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AreaPropertyTransparencyDemo
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Åtkomst till den första serien
            Aspose.Cells.Charts.Series series = chart.NSeries[0];

            // Demonstrera Transparency-egenskapen
            Console.WriteLine("Initial area transparency: " + series.Area.Transparency);
            Console.WriteLine("Initial border transparency: " + series.Border.Transparency);

            // Ändra transparensvärden
            series.Area.Transparency = 0.5; // 50% transparent
            series.Border.Transparency = 0.2; // 20% transparent

            Console.WriteLine("Modified area transparency: " + series.Area.Transparency);
            Console.WriteLine("Modified border transparency: " + series.Border.Transparency);

            // Spara arbetsboken
            workbook.Save("AreaPropertyTransparencyDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


