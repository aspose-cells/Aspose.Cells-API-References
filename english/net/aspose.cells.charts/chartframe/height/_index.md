---
title: ChartFrame.Height
second_title: Aspose.Cells for .NET API Reference
description: ChartFrame property. Gets or sets the height of frame in units of 1/4000 of the chart area
type: docs
url: /net/aspose.cells.charts/chartframe/height/
---
## ChartFrame.Height property

Gets or sets the height of frame in units of 1/4000 of the chart area.

```csharp
[Obsolete("Use ChartFrame.HeightRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int Height { get; set; }
```

### Remarks

How to convert units of 1/4000 to pixels? Height In Pixels = Y * Chart.ChartObject.Height / 4000d;

NOTE: This member is now obsolete. Please use ChartFrame.HeightRatioToChart property, instead. Height = HeightRatioToChart * 4000. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: AssertHelper.AreEqual(dlabelsSrc.Height, dlabelsDest.Height, info + ".Height");
public static void ChartFrame_Property_Height(DataLabels dlabelsSrc, DataLabels dlabelsDest, string info)
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
            LineTest.ChartFrame_Property_Height(dlabelsSrc.Border, dlabelsDest.Border, info + ".Border");
            AssertHelper.AreEqual(dlabelsSrc.Shadow, dlabelsDest.Shadow, info + ".Shadow");
            AreaTest.ChartFrame_Property_Height(dlabelsSrc.Area, dlabelsDest.Area, info + ".Area");
            //====================compare Font================//
            FontTest.ChartFrame_Property_Height(dlabelsSrc.TextFont, dlabelsDest.TextFont, info + ".TextFont");
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

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


