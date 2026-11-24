---
title: "SparklineGroup.VerticalAxisMinValueType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SparklineGroup-Eigenschaft. Stellt den Typ des minimalen Werts der vertikalen Achse dar."
type: docs
url: /de/net/aspose.cells.charts/sparklinegroup/verticalaxisminvaluetype/
---
## SparklineGroup.VerticalAxisMinValueType property

Stellt den Typ des minimalen Werts der vertikalen Achse dar.

```csharp
public SparklineAxisMinMaxType VerticalAxisMinValueType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyVerticalAxisMinValueTypeDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe und ein Arbeitsblatt
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);

            // Sparkline-Position definieren
            CellArea cellArea = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Sparkline-Gruppe hinzufügen
            int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, cellArea);
            SparklineGroup group = worksheet.SparklineGroups[groupIndex];
            group.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);

            // Vertikalen Achsen-Minimalwerttyp festlegen
            group.VerticalAxisMinValueType = SparklineAxisMinMaxType.AutoIndividual;

            // Speichere die Arbeitsmappe
            workbook.Save("SparklineVerticalAxisMinValueTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [SparklineAxisMinMaxType](../../sparklineaxisminmaxtype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


