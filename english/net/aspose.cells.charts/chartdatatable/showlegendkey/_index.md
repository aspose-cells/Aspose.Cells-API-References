---
title: ChartDataTable.ShowLegendKey
second_title: Aspose.Cells for .NET API Reference
description: ChartDataTable property. True if the data label legend key is visible
type: docs
url: /net/aspose.cells.charts/chartdatatable/showlegendkey/
---
## ChartDataTable.ShowLegendKey property

True if the data label legend key is visible.

```csharp
public bool ShowLegendKey { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(cdtableSrc.ShowLegendKey, cdtableDest.ShowLegendKey, info + ".ShowLegendKey");
public static void ChartDataTable_Property_ShowLegendKey(ChartDataTable cdtableSrc, ChartDataTable cdtableDest, string info)
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
            LineTest.ChartDataTable_Property_ShowLegendKey(cdtableSrc.Border, cdtableDest.Border, info + ".Border");
            
            AssertHelper.AreEqual(cdtableSrc.AutoScaleFont, cdtableDest.AutoScaleFont, info+".AutoScaleFont");
            FontTest.ChartDataTable_Property_ShowLegendKey(cdtableSrc.Font, cdtableDest.Font, info + ".Font");
            AssertHelper.AreEqual(cdtableSrc.BackgroundMode, cdtableDest.BackgroundMode, info+ ".BackgroundMode");
        }
```

### See Also

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


