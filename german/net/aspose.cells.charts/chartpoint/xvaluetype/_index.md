---
title: "ChartPoint.XValueType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Eigenschaft. Gibt den X-Werttyp des Diagrammpunkts zurück"
type: docs
url: /de/net/aspose.cells.charts/chartpoint/xvaluetype/
---
## ChartPoint.XValueType property

Ermittelt den Typ des X‑Werts des Diagrammpunkts.

```csharp
public CellValueType XValueType { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Den ersten Diagrammpunkt abrufen
            ChartPoint point = chart.NSeries[0].Points[0];

            // Zeigen Sie den aktuellen XValueType an
            Console.WriteLine("Current XValueType: " + point.XValueType);

            // Setzen Sie einen neuen XValue (dies aktualisiert automatisch den XValueType)
            point.XValue = DateTime.Now; // Changing to DateTime type
            Console.WriteLine("After setting DateTime value, XValueType: " + point.XValueType);

            point.XValue = "New Category"; // Changing to String type
            Console.WriteLine("After setting String value, XValueType: " + point.XValueType);

            point.XValue = 123.45; // Changing to Numeric type
            Console.WriteLine("After setting Numeric value, XValueType: " + point.XValueType);

            // Speichere die Arbeitsmappe
            workbook.Save("ChartPointXValueTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [CellValueType](../../../aspose.cells/cellvaluetype/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


