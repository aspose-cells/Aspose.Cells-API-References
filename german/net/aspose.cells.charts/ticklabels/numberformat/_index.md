---
title: "TickLabels.NumberFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TickLabels-Eigenschaft. Stellt die Formatzeichenfolge für das TickLabels-Objekt dar"
type: docs
url: /de/net/aspose.cells.charts/ticklabels/numberformat/
---
## TickLabels.NumberFormat property

Stellt die Formatzeichenfolge für das TickLabels‑Objekt dar.

```csharp
public string NumberFormat { get; set; }
```

### Hinweise

Die Formatzeichenfolge ist dieselbe wie eine benutzerdefinierte Formatzeichenfolge, die einer Zelle zugewiesen wird. Zum Beispiel, "$0".

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyNumberFormatDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(1.2345);
            worksheet.Cells["A3"].PutValue(2.3456);
            worksheet.Cells["A4"].PutValue(3.4567);

            // Ein Diagramm erstellen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("A2:A4", true);

            // Zahlenformat für Tick-Labels der Werteachse festlegen
            chart.ValueAxis.TickLabels.NumberFormat = "0.00";

            // Speichere die Arbeitsmappe
            workbook.Save("TickLabelsNumberFormatDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


