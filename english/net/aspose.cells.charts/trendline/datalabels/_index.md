---
title: Trendline.DataLabels
second_title: Aspose.Cells for .NET API Reference
description: Trendline property. Represents the DataLabels object for the specified series
type: docs
url: /net/aspose.cells.charts/trendline/datalabels/
---
## Trendline.DataLabels property

Represents the DataLabels object for the specified series.

```csharp
public DataLabels DataLabels { get; }
```

### Examples

```csharp
// Called: DataLabelsTest.equals(tlSrc.DataLabels, tlDest.DataLabels, info + ".DataLabels");
public static void Property_DataLabels(Trendline tlSrc, Trendline tlDest, string info)
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
                AssertHelper.Property_DataLabels(tlSrc.Color, tlDest.Color, info + ".Color");
                DataLabelsTest.Property_DataLabels(tlSrc.DataLabels, tlDest.DataLabels, info + ".DataLabels");
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

* class [DataLabels](../../datalabels/)
* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


