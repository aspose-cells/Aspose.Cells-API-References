---
title: Trendline.Backward
second_title: Aspose.Cells for .NET API Reference
description: Trendline property. Returns or sets the number of periods or units on a scatter chart that the trendline extends backward. The number of periods must be greater than or equal to zero. If the chart type is column the number of periods must be between 0 and 0.5
type: docs
url: /net/aspose.cells.charts/trendline/backward/
---
## Trendline.Backward property

Returns or sets the number of periods (or units on a scatter chart) that the trendline extends backward. The number of periods must be greater than or equal to zero. If the chart type is column ,the number of periods must be between 0 and 0.5

```csharp
public double Backward { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(tlSrc.Backward, tlDest.Backward, info + &amp;quot;.Backward&amp;quot;);
public static void Property_Backward(Trendline tlSrc, Trendline tlDest, string info)
        {
            if (AssertHelper.checkNull(tlSrc, tlDest, info))
            {
                return;
            }
            bool isvSrc = tlSrc.IsVisible;
            bool isvDest = tlDest.IsVisible;
            AssertHelper.AreEqual(isvSrc, isvDest, info + &quot;.IsVisible&quot;);
            if (isvSrc &amp;&amp; isvDest)
            {
                AssertHelper.AreEqual(tlSrc.Name, tlDest.Name, info + &quot;.Name&quot;);
                AssertHelper.AreEqual(tlSrc.Type, tlDest.Type, info + &quot;.Type&quot;);
                AssertHelper.AreEqual(tlSrc.Backward, tlDest.Backward, info + &quot;.Backward&quot;);
                AssertHelper.Property_Backward(tlSrc.Color, tlDest.Color, info + &quot;.Color&quot;);
                DataLabelsTest.Property_Backward(tlSrc.DataLabels, tlDest.DataLabels, info + &quot;.DataLabels&quot;);
                AssertHelper.AreEqual(tlSrc.DisplayEquation, tlDest.DisplayEquation, info + &quot;.DisplayEquation&quot;);
                AssertHelper.AreEqual(tlSrc.DisplayRSquared, tlDest.DisplayRSquared, info + &quot;.DisplayRSquared&quot;);
                AssertHelper.AreEqual(tlSrc.Forward, tlDest.Forward, delta, info + &quot;.Forward&quot;);
                AssertHelper.AreEqual(tlSrc.Intercept, tlDest.Intercept, delta, info + &quot;.Intercept&quot;);
                AssertHelper.AreEqual(tlSrc.IsNameAuto, tlDest.IsNameAuto, info + &quot;.IsNameAuto&quot;);
                AssertHelper.AreEqual(tlSrc.Order, tlDest.Order, info + &quot;.Order&quot;);
                AssertHelper.AreEqual(tlSrc.Period, tlDest.Period, info + &quot;.Period&quot;);
                AssertHelper.AreEqual(tlSrc.Style, tlDest.Style, info + &quot;.Style&quot;);
                AssertHelper.AreEqual(tlSrc.Weight, tlDest.Weight, info + &quot;.Weight&quot;);
            }

        }
```

### See Also

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


