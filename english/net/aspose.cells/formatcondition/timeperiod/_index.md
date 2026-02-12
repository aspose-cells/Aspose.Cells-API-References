---
title: FormatCondition.TimePeriod
second_title: Aspose.Cells for .NET API Reference
description: FormatCondition property. The applicable time period in a date occurrin conditional formatting rule. Valid only for type is timePeriod. The default value is TimePeriodType.Today
type: docs
url: /net/aspose.cells/formatcondition/timeperiod/
---
## FormatCondition.TimePeriod property

The applicable time period in a "date occurrin" conditional formatting rule. Valid only for type is timePeriod. The default value is TimePeriodType.Today.

```csharp
public TimePeriodType TimePeriod { get; set; }
```

### Examples

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

            // Add sample date values to demonstrate time period formatting
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

### See Also

* enum [TimePeriodType](../../timeperiodtype/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


