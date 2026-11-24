---
title: "Enum WeightType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.WeightType Enum. Enumeriert die Gewichtstypen für einen Bildrahmen oder eine Diagrammlinie"
type: docs
url: /de/net/aspose.cells.drawing/weighttype/
---
## WeightType enumeration

Enumeriert die Gewichtstypen für einen Bildrahmen oder eine Diagrammlinie.

```csharp
public enum WeightType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| HairLine | `-1` | Stellt das Gewicht einer Haarlinie dar. |
| MediumLine | `1` | Stellt das Gewicht einer Mittellinie dar. |
| SingleLine | `0` | Stellt das Gewicht einer Einzelinie dar. |
| WideLine | `2` | Stellt das Gewicht einer breiten Linie dar. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassWeightTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie ein Diagramm hinzu und erhalten Sie dessen Diagrammbereich
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 5, 15, 15);
            Chart chart = worksheet.Charts[chartIndex];
            ChartArea chartArea = chart.ChartArea;
            
            // Legen Sie den Randgewichtstyp fest
            chartArea.Border.Weight = WeightType.WideLine;
            
            // Überprüfen Sie den Gewichtstyp
            Console.WriteLine("Chart Area Border Weight: " + chartArea.Border.Weight);
            
            // Speichere die Arbeitsmappe
            workbook.Save("WeightTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


