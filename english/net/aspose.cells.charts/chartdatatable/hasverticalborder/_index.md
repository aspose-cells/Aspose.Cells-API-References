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
// Called: AssertHelper.AreEqual(cdtableSrc.HasVerticalBorder, cdtableDest.HasVerticalBorder, info + ".HasVerticalBorder");
public static void Property_HasVerticalBorder(ChartDataTable cdtableSrc, ChartDataTable cdtableDest, string info)
        {            
            if (AssertHelper.checkNull(cdtableSrc, cdtableDest, info))
            {
                return;
            }    
            //=========DataTable Options===============//
            AssertHelper.AreEqual(cdtableSrc.HasHorizontalBorder, cdtableDest.HasHorizontalBorder, info + ".HasHorizontalBorder");
            AssertHelper.AreEqual(cdtableSrc.HasVerticalBorder, cdtableDest.HasVerticalBorder, info + ".HasVerticalBorder");
            AssertHelper.AreEqual(cdtableSrc.HasOutlineBorder, cdtableDest.HasOutlineBorder, info + ".HasOutlineBorder");
            AssertHelper.AreEqual(cdtableSrc.ShowLegendKey, cdtableDest.ShowLegendKey, info + ".ShowLegendKey");
            //=========Fill==========================//            
            LineTest.Property_HasVerticalBorder(cdtableSrc.Border, cdtableDest.Border, info + ".Border");
            
            AssertHelper.AreEqual(cdtableSrc.AutoScaleFont, cdtableDest.AutoScaleFont, info+".AutoScaleFont");
            FontTest.Property_HasVerticalBorder(cdtableSrc.Font, cdtableDest.Font, info + ".Font");
            AssertHelper.AreEqual(cdtableSrc.BackgroundMode, cdtableDest.BackgroundMode, info+ ".BackgroundMode");
        }
```

### See Also

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


