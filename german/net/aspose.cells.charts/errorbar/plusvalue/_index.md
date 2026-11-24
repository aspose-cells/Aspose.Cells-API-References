---
title: "ErrorBar.PlusValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ErrorBar-Eigenschaft. Gibt den positiven Fehlerwert an, wenn der Fehlerbalkentyp benutzerdefiniert ist."
type: docs
url: /de/net/aspose.cells.charts/errorbar/plusvalue/
---
## ErrorBar.PlusValue property

Stellt den positiven Fehlermengenwert dar, wenn der Fehlermargen-Typ benutzerdefiniert ist.

```csharp
public string PlusValue { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ErrorBarPropertyPlusValueDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(5);
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(40);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);

            // Fehlerbalken konfigurieren
            ErrorBar errorBar = chart.NSeries[0].YErrorBar;
            errorBar.DisplayType = ErrorBarDisplayType.Both;
            errorBar.Type = ErrorBarType.Custom;
            errorBar.PlusValue = "=A2";  // Using PlusValue property
            errorBar.MinusValue = "=A3";

            // Speichere die Arbeitsmappe
            workbook.Save("ErrorBarPlusValueDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


