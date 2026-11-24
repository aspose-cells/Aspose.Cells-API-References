---
title: "SeriesLayoutProperties.IsIntervalLeftClosed"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SeriesLayoutProperties‑Eigenschaft. Gibt an, ob das Intervall auf der linken Seite geschlossen ist"
type: docs
url: /de/net/aspose.cells.charts/serieslayoutproperties/isintervalleftclosed/
---
## SeriesLayoutProperties.IsIntervalLeftClosed property

Gibt an, ob das Intervall auf der linken Seite geschlossen ist.

```csharp
public bool IsIntervalLeftClosed { get; set; }
```

### Hinweise

Nur für ParetoLine‑Diagramm.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyIsIntervalLeftClosedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B1"].PutValue(15);
            worksheet.Cells["B2"].PutValue(25);
            worksheet.Cells["B3"].PutValue(35);

            // Diagramm erstellen
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            int seriesIndex = chart.NSeries.Add("A1:B3", true);
            Aspose.Cells.Charts.Series series = chart.NSeries[seriesIndex];

            // Setze die IsIntervalLeftClosed‑Eigenschaft
            series.LayoutProperties.IsIntervalLeftClosed = true;

            // Arbeitsmappe speichern.
            workbook.Save("SeriesLayoutPropertiesIsIntervalLeftClosedDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


