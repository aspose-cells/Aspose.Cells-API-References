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
// Called: AssertHelper.AreEqual(tlSrc.Backward, tlDest.Backward, info + ".Backward");
public static void Property_Backward(Trendline tlSrc, Trendline tlDest, string info)
        {
            if (AssertHelper.checkNull(tlSrc, tlDest, info))
            {
                return;
            }
            bool isvSrc = tlSrc.IsVisible;
            bool isvDest = tlDest.IsVisible;
            AssertHelper.AreEqual(isvSrc, isvDest, info + ".IsVisible");
            if (isvSrc && isvDest)
            {
                AssertHelper.AreEqual(tlSrc.Name, tlDest.Name, info + ".Name");
                AssertHelper.AreEqual(tlSrc.Type, tlDest.Type, info + ".Type");
                AssertHelper.AreEqual(tlSrc.Backward, tlDest.Backward, info + ".Backward");
                AssertHelper.Property_Backward(tlSrc.Color, tlDest.Color, info + ".Color");
                DataLabelsTest.Property_Backward(tlSrc.DataLabels, tlDest.DataLabels, info + ".DataLabels");
                AssertHelper.AreEqual(tlSrc.DisplayEquation, tlDest.DisplayEquation, info + ".DisplayEquation");
                AssertHelper.AreEqual(tlSrc.DisplayRSquared, tlDest.DisplayRSquared, info + ".DisplayRSquared");
                AssertHelper.AreEqual(tlSrc.Forward, tlDest.Forward, delta, info + ".Forward");
                AssertHelper.AreEqual(tlSrc.Intercept, tlDest.Intercept, delta, info + ".Intercept");
                AssertHelper.AreEqual(tlSrc.IsNameAuto, tlDest.IsNameAuto, info + ".IsNameAuto");
                AssertHelper.AreEqual(tlSrc.Order, tlDest.Order, info + ".Order");
                AssertHelper.AreEqual(tlSrc.Period, tlDest.Period, info + ".Period");
                AssertHelper.AreEqual(tlSrc.Style, tlDest.Style, info + ".Style");
                AssertHelper.AreEqual(tlSrc.Weight, tlDest.Weight, info + ".Weight");
            }

        }
```

### See Also

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


