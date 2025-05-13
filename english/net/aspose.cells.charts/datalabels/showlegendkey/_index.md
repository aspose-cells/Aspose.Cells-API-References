---
title: DataLabels.ShowLegendKey
second_title: Aspose.Cells for .NET API Reference
description: DataLabels property. Represents a specified charts data label legend key display behavior. True if the data label legend key is visible
type: docs
url: /net/aspose.cells.charts/datalabels/showlegendkey/
---
## DataLabels.ShowLegendKey property

Represents a specified chart's data label legend key display behavior. True if the data label legend key is visible.

```csharp
public bool ShowLegendKey { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(dlabelsSrc.ShowLegendKey, dlabelsDest.ShowLegendKey, info + ".ShowLegendKey");
public static void DataLabels_Property_ShowLegendKey(DataLabels dlabelsSrc, DataLabels dlabelsDest, string info)
        {
            if (AssertHelper.checkNull(dlabelsSrc, dlabelsDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(dlabelsSrc.ShowSeriesName, dlabelsDest.ShowSeriesName, info + ".ShowSeriesName");
            AssertHelper.AreEqual(dlabelsSrc.ShowCategoryName, dlabelsDest.ShowCategoryName, info + ".ShowCategoryName");
            AssertHelper.AreEqual(dlabelsSrc.ShowValue, dlabelsDest.ShowValue, info + ".ShowValue");
            AssertHelper.AreEqual(dlabelsSrc.ShowPercentage, dlabelsDest.ShowPercentage, info + ".ShowPercentage");
            AssertHelper.AreEqual(dlabelsSrc.ShowBubbleSize, dlabelsDest.ShowBubbleSize, info + ".ShowBubbleSize");
            AssertHelper.AreEqual(dlabelsSrc.SeparatorType, dlabelsDest.SeparatorType, info + ".Separator");
            AssertHelper.AreEqual(dlabelsSrc.ShowLegendKey, dlabelsDest.ShowLegendKey, info + ".ShowLegendKey");
            //====================compare Patterns================//
            LineTest.DataLabels_Property_ShowLegendKey(dlabelsSrc.Border, dlabelsDest.Border, info + ".Border");
            AssertHelper.AreEqual(dlabelsSrc.Shadow, dlabelsDest.Shadow, info + ".Shadow");
            AreaTest.DataLabels_Property_ShowLegendKey(dlabelsSrc.Area, dlabelsDest.Area, info + ".Area");
            //====================compare Font================//
            FontTest.DataLabels_Property_ShowLegendKey(dlabelsSrc.TextFont, dlabelsDest.TextFont, info + ".TextFont");
            AssertHelper.AreEqual(dlabelsSrc.AutoScaleFont, dlabelsDest.AutoScaleFont, info + ".AutoScaleFont");
            AssertHelper.AreEqual(dlabelsSrc.BackgroundMode, dlabelsDest.BackgroundMode, info + ".BackgroundMode");
            //====================compare Number================//
            bool lSrc = dlabelsSrc.NumberFormatLinked;
            bool lDest = dlabelsDest.NumberFormatLinked;
            AssertHelper.AreEqual(lSrc, lDest, info + ".NumberFormatLinked");
            if (lSrc == false && lDest == false)
            {
                AssertHelper.AreEqual(dlabelsSrc.Number, dlabelsDest.Number, info + ".Number");
                AssertHelper.AreEqual(dlabelsSrc.NumberFormat, dlabelsDest.NumberFormat, info + ".NumberFormat");
            }
            //====================compare Alignment================//
            AssertHelper.AreEqual(dlabelsSrc.TextHorizontalAlignment, dlabelsDest.TextHorizontalAlignment, info + ".TextHorizontalAlignment");
            AssertHelper.AreEqual(dlabelsSrc.TextVerticalAlignment, dlabelsDest.TextVerticalAlignment, info + ".TextVerticalAlignment");
            AssertHelper.AreEqual(dlabelsSrc.Position, dlabelsDest.Position, info + ".Position");
            AssertHelper.AreEqual(dlabelsSrc.TextDirection, dlabelsDest.TextDirection, info + ".TextDirection");
            AssertHelper.AreEqual(dlabelsSrc.RotationAngle, dlabelsDest.RotationAngle, info + ".RotationAngle");      
            //====================compare other===================//
            AssertHelper.AreEqual(dlabelsSrc.Height, dlabelsDest.Height, info + ".Height");
            AssertHelper.AreEqual(dlabelsSrc.Width, dlabelsDest.Width, info + ".Width");            
        }
```

### See Also

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


