---
title: "ChartPoint.YValueType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Eigenschaft. Gibt den Y‑Werttyp des ChartPoint zurück."
type: docs
url: /de/net/aspose.cells.charts/chartpoint/yvaluetype/
---
## ChartPoint.YValueType property

Ermittelt den Typ des Y‑Werts des Diagrammpunkts.

```csharp
public CellValueType YValueType { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyYValueTypeDemo
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

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Den ersten Diagrammpunkt in der ersten Serie abrufen
            ChartPoint chartPoint = chart.NSeries[0].Points[0];

            // Zeige den aktuellen YValueType an.
            Console.WriteLine("Current YValueType: " + chartPoint.YValueType);

            // Zeige den YValue vor der Änderung
            Console.WriteLine("Current YValue: " + chartPoint.YValue);

            // Ändere den YValue zu einem anderen Typ (String, um den Typwechsel zu demonstrieren)
            chartPoint.YValue = "15"; // This will change the YValueType to IsString

            // Zeige den YValueType nach der Änderung
            Console.WriteLine("New YValueType: " + chartPoint.YValueType);
            Console.WriteLine("New YValue: " + chartPoint.YValue);

            // Speichere die Arbeitsmappe
            workbook.Save("ChartPointPropertyYValueTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [CellValueType](../../../aspose.cells/cellvaluetype/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


