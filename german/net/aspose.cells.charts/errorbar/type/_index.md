---
title: "ErrorBar.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ErrorBar-Eigenschaft. Gibt den Typ des Fehlerbalkenbetrags an."
type: docs
url: /de/net/aspose.cells.charts/errorbar/type/
---
## ErrorBar.Type property

Stellt den Betragstyp der Fehlermarge dar.

```csharp
public ErrorBarType Type { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ErrorBarPropertyTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            ws.Cells["A1"].PutValue(5);
            ws.Cells["A2"].PutValue(3);
            
            // Ein Diagramm erstellen
            int chartIndex = ws.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = ws.Charts[chartIndex];
            
            // Seriendaten hinzufügen
            chart.NSeries.Add("A3:A10", true);
            Series series = chart.NSeries[0];
            
            // Benutzerdefinierten Fehlerbalkentyp und Werte festlegen
            series.YErrorBar.Type = ErrorBarType.Custom;
            series.YErrorBar.PlusValue = "=Sheet1!A1";
            series.YErrorBar.MinusValue = "=Sheet1!A2";
            
            // Speichere die Arbeitsmappe
            wb.Save("ErrorBarDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ErrorBarType](../../errorbartype/)
* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


