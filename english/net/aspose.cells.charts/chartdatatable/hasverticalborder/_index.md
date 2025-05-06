---
title: ChartDataTable.HasVerticalBorder
second_title: Aspose.Cells for .NET API Reference
description: ChartDataTable property. True if the chart data table has vertical cell borders
type: docs
url: /net/aspose.cells.charts/chartdatatable/hasverticalborder/
---
## ChartDataTable.HasVerticalBorder property

True if the chart data table has vertical cell borders

```csharp
public bool HasVerticalBorder { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(cdtableSrc.HasVerticalBorder, cdtableDest.HasVerticalBorder, info + &amp;quot;.HasVerticalBorder&amp;quot;);
public static void Property_HasVerticalBorder(ChartDataTable cdtableSrc, ChartDataTable cdtableDest, string info)
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
            LineTest.Property_HasVerticalBorder(cdtableSrc.Border, cdtableDest.Border, info + &quot;.Border&quot;);
            
            AssertHelper.AreEqual(cdtableSrc.AutoScaleFont, cdtableDest.AutoScaleFont, info+&quot;.AutoScaleFont&quot;);
            FontTest.Property_HasVerticalBorder(cdtableSrc.Font, cdtableDest.Font, info + &quot;.Font&quot;);
            AssertHelper.AreEqual(cdtableSrc.BackgroundMode, cdtableDest.BackgroundMode, info+ &quot;.BackgroundMode&quot;);
        }
```

### See Also

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


