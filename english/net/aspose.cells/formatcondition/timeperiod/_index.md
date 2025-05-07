---
title: FormatCondition.TimePeriod
second_title: Aspose.Cells for .NET API Reference
description: FormatCondition property. The applicable time period in a date occurring conditional formatting rule. Valid only for type  timePeriod. The default value is TimePeriodType.Today
type: docs
url: /net/aspose.cells/formatcondition/timeperiod/
---
## FormatCondition.TimePeriod property

The applicable time period in a "date occurring…" conditional formatting rule. Valid only for type = timePeriod. The default value is TimePeriodType.Today.

```csharp
public TimePeriodType TimePeriod { get; set; }
```

### Examples

```csharp
// Called: fc.TimePeriod = TimePeriodType.Today;
public static void Property_TimePeriod()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a conditional formatting rule
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Define the cell area for the conditional formatting
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Add a condition for the time period
            int conditionIndex = fcs.AddCondition(FormatConditionType.TimePeriod);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.LightBlue;

            // Set the time period type
            fc.TimePeriod = TimePeriodType.Today;

            // Save the workbook
            workbook.Save("TimePeriodTypeExample.xlsx");

            return;
        }
```

### See Also

* enum [TimePeriodType](../../timeperiodtype/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


