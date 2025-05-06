---
title: ChartDataTable.HasHorizontalBorder
second_title: Aspose.Cells for .NET API Reference
description: ChartDataTable property. True if the chart data table has horizontal cell borders
type: docs
url: /net/aspose.cells.charts/chartdatatable/hashorizontalborder/
---
## ChartDataTable.HasHorizontalBorder property

True if the chart data table has horizontal cell borders

```csharp
public bool HasHorizontalBorder { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(cdtableSrc.HasHorizontalBorder, cdtableDest.HasHorizontalBorder, info + &amp;quot;.HasHorizontalBorder&amp;quot;);
public static void Property_HasHorizontalBorder(ChartDataTable cdtableSrc, ChartDataTable cdtableDest, string info)
        {            
            if (AssertHelper.checkNull(cdtableSrc, cdtableDest, info))
            {
                return;
            }    
            //=========DataTable Options===============//
            AssertHelper.AreEqual(cdtableSrc.HasHorizontalBorder, cdtableDest.HasHorizontalBorder, info + &quot;.HasHorizontalBorder&quot;);
            AssertHelper.AreEqual(cdtableSrc.HasVerticalBorder, cdtableDest.HasVerticalBorder, info + &quot;.HasVerticalBorder&quot;);
            AssertHelper.AreEqual(cdtableSrc.HasOutlineBorder, cdtableDest.HasOutlineBorder, info + &quot;.HasOutlineBorder&quot;);
            AssertHelper.AreEqual(cdtableSrc.ShowLegendKey, cdtableDest.ShowLegendKey, info + &quot;.ShowLegendKey&quot;);
            //=========Fill==========================//            
            LineTest.Property_HasHorizontalBorder(cdtableSrc.Border, cdtableDest.Border, info + &quot;.Border&quot;);
            
            AssertHelper.AreEqual(cdtableSrc.AutoScaleFont, cdtableDest.AutoScaleFont, info+&quot;.AutoScaleFont&quot;);
            FontTest.Property_HasHorizontalBorder(cdtableSrc.Font, cdtableDest.Font, info + &quot;.Font&quot;);
            AssertHelper.AreEqual(cdtableSrc.BackgroundMode, cdtableDest.BackgroundMode, info+ &quot;.BackgroundMode&quot;);
        }
```

### See Also

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


