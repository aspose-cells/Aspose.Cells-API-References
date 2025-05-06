---
title: AboveAverage.IsEqualAverage
second_title: Aspose.Cells for .NET API Reference
description: AboveAverage property. Get or set the flag indicating whether the aboveAverage and belowAverage criteria is inclusive of the average itself or exclusive of that value. true indicates to include the average value in the criteria. Default value is false
type: docs
url: /net/aspose.cells/aboveaverage/isequalaverage/
---
## AboveAverage.IsEqualAverage property

Get or set the flag indicating whether the 'aboveAverage' and 'belowAverage' criteria is inclusive of the average itself, or exclusive of that value. 'true' indicates to include the average value in the criteria. Default value is false.

```csharp
public bool IsEqualAverage { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(formatSrc.AboveAverage.IsEqualAverage, formatDest.AboveAverage.IsEqualAverage, info + &amp;quot;.AboveAverage.IsEqualAverage&amp;quot;);
public static void Property_IsEqualAverage(FormatCondition formatSrc, FormatCondition formatDest, string info)
        {
            if (AssertHelper.checkNull(formatSrc, formatDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(formatSrc.Type, formatDest.Type, info + &quot;.Type&quot;);
            AssertHelper.AreEqual(formatSrc.Operator, formatDest.Operator, info + &quot;.Operator&quot;);
            AssertHelper.AreEqual(formatSrc.Style, formatDest.Style, info + &quot;.Style&quot;);

            switch (formatSrc.Type)
            {
                case FormatConditionType.AboveAverage:
                    AssertHelper.AreEqual(formatSrc.AboveAverage.IsAboveAverage, formatDest.AboveAverage.IsAboveAverage, info + &quot;.AboveAverage.IsAboveAverage&quot;);
                    AssertHelper.AreEqual(formatSrc.AboveAverage.IsEqualAverage, formatDest.AboveAverage.IsEqualAverage, info + &quot;.AboveAverage.IsEqualAverage&quot;);
                    AssertHelper.AreEqual(formatSrc.AboveAverage.StdDev, formatDest.AboveAverage.StdDev, info + &quot;.AboveAverage.StdDev&quot;);
                    break;
                case FormatConditionType.ColorScale:
                    equals(formatSrc.ColorScale, formatDest.ColorScale, info + &quot;.ColorScale&quot;);
                    break;
                case FormatConditionType.DataBar:
                    equals(formatSrc.DataBar, formatDest.DataBar, info + &quot;.DataBar&quot;);
                    break;
                case FormatConditionType.IconSet:
                    equals(formatSrc.IconSet, formatDest.IconSet, info + &quot;.IconSet&quot;);
                    break;
                case FormatConditionType.TimePeriod:
                    AssertHelper.AreEqual(formatSrc.TimePeriod, formatDest.TimePeriod, info + &quot;.TimePeriod&quot;);
                    break;
                case FormatConditionType.Top10:
                    AssertHelper.AreEqual(formatSrc.Top10.IsBottom, formatDest.Top10.IsBottom, info + &quot;.Top10.IsBottom&quot;);
                    AssertHelper.AreEqual(formatSrc.Top10.IsPercent, formatDest.Top10.IsPercent, info + &quot;.Top10.IsPercent&quot;);
                    AssertHelper.AreEqual(formatSrc.Top10.Rank, formatDest.Top10.Rank, info + &quot;.Top10.Rank&quot;);
                    break;               
            }            

        }
```

### See Also

* class [AboveAverage](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


