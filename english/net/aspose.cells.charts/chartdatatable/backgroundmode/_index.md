---
title: ChartDataTable.BackgroundMode
second_title: Aspose.Cells for .NET API Reference
description: ChartDataTable property. Gets and sets the display mode of the background
type: docs
url: /net/aspose.cells.charts/chartdatatable/backgroundmode/
---
## ChartDataTable.BackgroundMode property

Gets and sets the display mode of the background

```csharp
public BackgroundMode BackgroundMode { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(cdtableSrc.BackgroundMode, cdtableDest.BackgroundMode, info+ &amp;quot;.BackgroundMode&amp;quot;);
public static void Property_BackgroundMode(ChartDataTable cdtableSrc, ChartDataTable cdtableDest, string info)
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
            LineTest.Property_BackgroundMode(cdtableSrc.Border, cdtableDest.Border, info + &quot;.Border&quot;);
            
            AssertHelper.AreEqual(cdtableSrc.AutoScaleFont, cdtableDest.AutoScaleFont, info+&quot;.AutoScaleFont&quot;);
            FontTest.Property_BackgroundMode(cdtableSrc.Font, cdtableDest.Font, info + &quot;.Font&quot;);
            AssertHelper.AreEqual(cdtableSrc.BackgroundMode, cdtableDest.BackgroundMode, info+ &quot;.BackgroundMode&quot;);
        }
```

### See Also

* enum [BackgroundMode](../../backgroundmode/)
* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


