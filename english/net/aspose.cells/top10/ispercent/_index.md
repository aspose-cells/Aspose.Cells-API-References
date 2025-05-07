---
title: Top10.IsPercent
second_title: Aspose.Cells for .NET API Reference
description: Top10 property. Get or set whether a top/bottom n rule is a top/bottom n percent rule. Default value is false
type: docs
url: /net/aspose.cells/top10/ispercent/
---
## Top10.IsPercent property

Get or set whether a "top/bottom n" rule is a "top/bottom n percent" rule. Default value is false.

```csharp
public bool IsPercent { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(formatSrc.Top10.IsPercent, formatDest.Top10.IsPercent, info + ".Top10.IsPercent");
public static void Property_IsPercent(FormatCondition formatSrc, FormatCondition formatDest, string info)
        {
            if (AssertHelper.checkNull(formatSrc, formatDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(formatSrc.Type, formatDest.Type, info + ".Type");
            AssertHelper.AreEqual(formatSrc.Operator, formatDest.Operator, info + ".Operator");
            AssertHelper.AreEqual(formatSrc.Style, formatDest.Style, info + ".Style");

            switch (formatSrc.Type)
            {
                case FormatConditionType.AboveAverage:
                    AssertHelper.AreEqual(formatSrc.AboveAverage.IsAboveAverage, formatDest.AboveAverage.IsAboveAverage, info + ".AboveAverage.IsAboveAverage");
                    AssertHelper.AreEqual(formatSrc.AboveAverage.IsEqualAverage, formatDest.AboveAverage.IsEqualAverage, info + ".AboveAverage.IsEqualAverage");
                    AssertHelper.AreEqual(formatSrc.AboveAverage.StdDev, formatDest.AboveAverage.StdDev, info + ".AboveAverage.StdDev");
                    break;
                case FormatConditionType.ColorScale:
                    equals(formatSrc.ColorScale, formatDest.ColorScale, info + ".ColorScale");
                    break;
                case FormatConditionType.DataBar:
                    equals(formatSrc.DataBar, formatDest.DataBar, info + ".DataBar");
                    break;
                case FormatConditionType.IconSet:
                    equals(formatSrc.IconSet, formatDest.IconSet, info + ".IconSet");
                    break;
                case FormatConditionType.TimePeriod:
                    AssertHelper.AreEqual(formatSrc.TimePeriod, formatDest.TimePeriod, info + ".TimePeriod");
                    break;
                case FormatConditionType.Top10:
                    AssertHelper.AreEqual(formatSrc.Top10.IsBottom, formatDest.Top10.IsBottom, info + ".Top10.IsBottom");
                    AssertHelper.AreEqual(formatSrc.Top10.IsPercent, formatDest.Top10.IsPercent, info + ".Top10.IsPercent");
                    AssertHelper.AreEqual(formatSrc.Top10.Rank, formatDest.Top10.Rank, info + ".Top10.Rank");
                    break;               
            }            

        }
```

### See Also

* class [Top10](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


