---
title: ChartDataTable.Font
second_title: Aspose.Cells for .NET API Reference
description: ChartDataTable property. Gets a Font object which represents the font setting of the specified chart data table
type: docs
url: /net/aspose.cells.charts/chartdatatable/font/
---
## ChartDataTable.Font property

Gets a `Font` object which represents the font setting of the specified chart data table.

```csharp
public Font Font { get; }
```

### Examples

```csharp
// Called: FontTest.equals(cdtableSrc.Font, cdtableDest.Font, info + &amp;quot;.Font&amp;quot;);
public static void Property_Font(ChartDataTable cdtableSrc, ChartDataTable cdtableDest, string info)
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
            LineTest.Property_Font(cdtableSrc.Border, cdtableDest.Border, info + &quot;.Border&quot;);
            
            AssertHelper.AreEqual(cdtableSrc.AutoScaleFont, cdtableDest.AutoScaleFont, info+&quot;.AutoScaleFont&quot;);
            FontTest.Property_Font(cdtableSrc.Font, cdtableDest.Font, info + &quot;.Font&quot;);
            AssertHelper.AreEqual(cdtableSrc.BackgroundMode, cdtableDest.BackgroundMode, info+ &quot;.BackgroundMode&quot;);
        }
```

### See Also

* class [Font](../../../aspose.cells/font/)
* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


