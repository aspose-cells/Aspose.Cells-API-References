---
title: "ChartPoint.XValueType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint egenskap. Hämtar X‑värdetyp för diagrampunkten"
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/xvaluetype/
---
## ChartPoint.XValueType property

Hämtar X‑värdestypen för diagrampunkten.

```csharp
public CellValueType XValueType { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyXValueTypeDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Hämta den första diagrampunkten
            ChartPoint point = chart.NSeries[0].Points[0];

            // Visa den aktuella XValueType
            Console.WriteLine("Current XValueType: " + point.XValueType);

            // Ställ in nytt XValue (detta kommer automatiskt att uppdatera XValueType)
            point.XValue = DateTime.Now; // Changing to DateTime type
            Console.WriteLine("After setting DateTime value, XValueType: " + point.XValueType);

            point.XValue = "New Category"; // Changing to String type
            Console.WriteLine("After setting String value, XValueType: " + point.XValueType);

            point.XValue = 123.45; // Changing to Numeric type
            Console.WriteLine("After setting Numeric value, XValueType: " + point.XValueType);

            // Spara arbetsboken
            workbook.Save("ChartPointXValueTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [CellValueType](../../../aspose.cells/cellvaluetype/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


