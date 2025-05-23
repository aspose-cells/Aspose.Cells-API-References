---
title: SeriesCollection.SecondCategoryData
second_title: Aspose.Cells for .NET API Reference
description: SeriesCollection property. Gets or sets the range of second category Axis values. It can be a range of cells such as d1e10 or a sequence of values such as26810. Only effects when some ASerieses plot on the second axis
type: docs
url: /net/aspose.cells.charts/seriescollection/secondcategorydata/
---
## SeriesCollection.SecondCategoryData property

Gets or sets the range of second category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). Only effects when some ASerieses plot on the second axis.

```csharp
public string SecondCategoryData { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(nseriesSrc.SecondCategoryData, nseriesDest.SecondCategoryData, info + ".SecondCategoryData");
public static void SeriesCollection_Property_SecondCategoryData(SeriesCollection nseriesSrc, SeriesCollection nseriesDest, string info)
        {
            if (AssertHelper.checkNull(nseriesSrc, nseriesDest, info))
            {
                return;
            }
            int countSrc = nseriesSrc.Count;
            int countDest = nseriesDest.Count;
            AssertHelper.AreEqual(countSrc, countDest, info + ".Count");
            for (int i = 0; i < countSrc && i < countDest; i++)
            {
                AssertHelper.AreEqual(nseriesSrc.CategoryData, nseriesDest.CategoryData, info + ".CategoryData");
                AssertHelper.AreEqual(nseriesSrc.IsColorVaried, nseriesDest.IsColorVaried, info + ".IsColorVaried");
                AssertHelper.AreEqual(nseriesSrc.SecondCategoryData, nseriesDest.SecondCategoryData, info + ".SecondCategoryData");
                ASeriesTest.SeriesCollection_Property_SecondCategoryData(nseriesSrc[i], nseriesDest[i], info + "[" + i + "]");
            }
        }
```

### See Also

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


