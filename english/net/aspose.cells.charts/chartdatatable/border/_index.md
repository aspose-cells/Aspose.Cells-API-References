---
title: ChartDataTable.Border
second_title: Aspose.Cells for .NET API Reference
description: ChartDataTable property. Returns a Border object that represents the border of the object
type: docs
url: /net/aspose.cells.charts/chartdatatable/border/
---
## ChartDataTable.Border property

Returns a Border object that represents the border of the object

```csharp
public Line Border { get; }
```

### Examples

```csharp
// Called: LineTest.equals(cdtableSrc.Border, cdtableDest.Border, info + ".Border");
public static void ChartDataTable_Property_Border(ChartDataTable cdtableSrc, ChartDataTable cdtableDest, string info)
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
            LineTest.ChartDataTable_Property_Border(cdtableSrc.Border, cdtableDest.Border, info + ".Border");
            
            AssertHelper.AreEqual(cdtableSrc.AutoScaleFont, cdtableDest.AutoScaleFont, info+".AutoScaleFont");
            FontTest.ChartDataTable_Property_Border(cdtableSrc.Font, cdtableDest.Font, info + ".Font");
            AssertHelper.AreEqual(cdtableSrc.BackgroundMode, cdtableDest.BackgroundMode, info+ ".BackgroundMode");
        }
```

### See Also

* class [Line](../../../aspose.cells.drawing/line/)
* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


