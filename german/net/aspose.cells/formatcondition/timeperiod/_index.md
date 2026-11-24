---
title: "FormatCondition.TimePeriod"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormatCondition-Eigenschaft. Der anwendbare Zeitraum in einer datumsbasierten bedingten Formatierungsregel. Nur gültig für den Typ timePeriod. Der Standardwert ist TimePeriodType.Today."
type: docs
url: /de/net/aspose.cells/formatcondition/timeperiod/
---
## FormatCondition.TimePeriod property

Der anwendbare Zeitraum in einer "date occurrin"-Regel für bedingte Formatierung. Gültig nur für Typ = timePeriod. Der Standardwert ist TimePeriodType.Today.

```csharp
public TimePeriodType TimePeriod { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyTimePeriodDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispiel-Datumswerte hinzu, um die Formatierung des Zeitraums zu demonstrieren.
            worksheet.Cells["A1"].PutValue(DateTime.Now);
            worksheet.Cells["A2"].PutValue(DateTime.Now.AddDays(-1));
            worksheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));

            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(area);

            int conditionIndex = fcs.AddCondition(FormatConditionType.TimePeriod);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.LightBlue;
            fc.TimePeriod = TimePeriodType.Today;

            workbook.Save("TimePeriodDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [TimePeriodType](../../timeperiodtype/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


