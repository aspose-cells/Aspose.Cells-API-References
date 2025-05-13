---
title: DataLabels.BackgroundMode
second_title: Aspose.Cells for .NET API Reference
description: DataLabels property. Gets and sets the display mode of the background
type: docs
url: /net/aspose.cells.charts/datalabels/backgroundmode/
---
## DataLabels.BackgroundMode property

Gets and sets the display mode of the background

```csharp
public BackgroundMode BackgroundMode { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(dlabelsSrc.BackgroundMode, dlabelsDest.BackgroundMode, info + ".BackgroundMode");
public static void DataLabels_Property_BackgroundMode(DataLabels dlabelsSrc, DataLabels dlabelsDest, string info)
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
            LineTest.DataLabels_Property_BackgroundMode(dlabelsSrc.Border, dlabelsDest.Border, info + ".Border");
            AssertHelper.AreEqual(dlabelsSrc.Shadow, dlabelsDest.Shadow, info + ".Shadow");
            AreaTest.DataLabels_Property_BackgroundMode(dlabelsSrc.Area, dlabelsDest.Area, info + ".Area");
            //====================compare Font================//
            FontTest.DataLabels_Property_BackgroundMode(dlabelsSrc.TextFont, dlabelsDest.TextFont, info + ".TextFont");
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

* enum [BackgroundMode](../../backgroundmode/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


