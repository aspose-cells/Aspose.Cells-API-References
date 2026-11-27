---
title: "Axis.CustUnit"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Axis-egenskap. Anger ett anpassat värde för visningsenheten"
type: docs
url: /sv/net/aspose.cells.charts/axis/custunit/
---
## Axis.CustUnit property

Anger ett anpassat värde för visningsenheten.

```csharp
[Obsolete("Use Axis.CustomUnit property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int CustUnit { get; set; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd istället Axis.CustomUnit property. Denna egenskap kommer att tas bort 12 månader senare sedan januari 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisPropertyCustUnitDemo
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
            worksheet.Cells["A5"].PutValue("D");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(1000000);
            worksheet.Cells["B3"].PutValue(2000000);
            worksheet.Cells["B4"].PutValue(3000000);
            worksheet.Cells["B5"].PutValue(4000000);

            // Lägg till ett diagram och ange dess dataintervall
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Hämta värdeaxeln
            Axis valueAxis = chart.ValueAxis;

            // Visa aktuellt CustUnit‑värde (föråldrad egenskap)
            Console.WriteLine("Current CustUnit value: " + valueAxis.CustUnit);

            // Ange ett nytt anpassat enhetsvärde (1,000,000)
            valueAxis.CustUnit = 1000000;
            valueAxis.IsDisplayUnitLabelShown = true;

            // Visa det nya CustUnit‑värdet
            Console.WriteLine("New CustUnit value: " + valueAxis.CustUnit);

            // Spara resultatet
            workbook.Save("AxisPropertyCustUnitDemo.xlsx");
        }
    }
}
```

### Se även

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


