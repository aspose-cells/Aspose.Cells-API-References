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
// Called: fcs[0].TimePeriod = TimePeriodType.LastMonth;
[Test]
        public void Property_TimePeriod()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells[&quot;A1&quot;].PutValue(&quot;2014/12/1&quot;, true);
            workbook.Worksheets[0].ConditionalFormattings.Add();
            FormatConditionCollection fcs = workbook.Worksheets[0].ConditionalFormattings[0];
            fcs.Add(CellArea.CreateCellArea(&quot;A1&quot;, &quot;A1&quot;), FormatConditionType.TimePeriod, OperatorType.None, null, null);
            fcs[0].TimePeriod = TimePeriodType.LastMonth;
            fcs[0].Style.ForegroundColor = Color.Red;
            Assert.AreEqual(cells[&quot;A1&quot;].GetDisplayStyle().ForegroundColor.ToArgb()&amp;0xFFFFFF,0);

        }
```

### See Also

* enum [TimePeriodType](../../timeperiodtype/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


