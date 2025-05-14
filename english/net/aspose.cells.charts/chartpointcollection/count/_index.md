---
title: ChartPointCollection.Count
second_title: Aspose.Cells for .NET API Reference
description: ChartPointCollection property. Gets the count of the chart point
type: docs
url: /net/aspose.cells.charts/chartpointcollection/count/
---
## ChartPointCollection.Count property

Gets the count of the chart point.

```csharp
public int Count { get; }
```

### Examples

```csharp
// Called: int countDest = cpointsDest.Count;
public static void ChartPointCollection_Property_Count(ChartType type, ChartPointCollection cpointsSrc, ChartPointCollection cpointsDest, string info)
        {
            if (AssertHelper.checkNull(cpointsSrc, cpointsDest, info))
            {
                return;
            }
            int countSrc = cpointsSrc.Count;
            int countDest = cpointsDest.Count;
            AssertHelper.AreEqual(countSrc, countDest, info + ".Count");
            for (int i = 0; i < countSrc && i < countDest; i++)
            {
                ChartPointCollection_Property_Count(type, cpointsSrc[i], cpointsDest[i], info);
            }

        }
```

### See Also

* class [ChartPointCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


