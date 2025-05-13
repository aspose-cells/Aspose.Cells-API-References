---
title: ChartArea.Width
second_title: Aspose.Cells for .NET API Reference
description: ChartArea property. Gets or sets the horizontal offset from its lower right corner column in units of 1/4000 of the chart area
type: docs
url: /net/aspose.cells.charts/chartarea/width/
---
## ChartArea.Width property

Gets or sets the horizontal offset from its lower right corner column, in units of 1/4000 of the chart area.

```csharp
[Obsolete("Use ChartArea.WidthRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Width { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Please use ChartArea.WidthRatioToChart property, instead. Width = WidthRatioToChart * 4000. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: AssertHelper.AreEqual(areaSrc.Width, areaDest.Width, info + ".Width");
public static void ChartArea_Property_Width(ChartArea areaSrc, ChartArea areaDest, string info)
        {
            if (AssertHelper.checkNull(areaSrc, areaDest, info))
            {
                return;
            }
            //============compare patterns==============//
            //border
            AssertHelper.AreEqual(areaSrc.Border.IsAuto, areaDest.Border.IsAuto, info + ".Border.IsAuto");
            AssertHelper.AreEqual(areaSrc.Border.IsVisible, areaDest.Border.IsVisible, info + ".Border.IsVisible");
            if (areaSrc.Border.IsVisible == true && areaSrc.Border.IsAuto == false)
            {
                //AssertHelper.AreEqual(areaSrc.Border.Style, areaDest.Border.Style, info + ".Border.Style");
                //AssertHelper.ChartArea_Property_Width(areaSrc.Border.Color, areaDest.Border.Color, info + ".Border.Color");
                //AssertHelper.AreEqual(areaSrc.Border.Weight, areaDest.Border.Weight, info + ".Border.Weight");
                LineTest.ChartArea_Property_Width(areaSrc.Border, areaDest.Border, info+".Border");
            }
            AssertHelper.AreEqual(areaSrc.Shadow, areaDest.Shadow, info + ".Shadow");
            //area
            AreaTest.ChartArea_Property_Width(areaSrc.Area, areaDest.Area, info + ".Area");
            //==============compare font================//
            FontTest.ChartArea_Property_Width(areaSrc.TextFont, areaDest.TextFont, info + ".TextFont");
            AssertHelper.AreEqual(areaSrc.AutoScaleFont, areaDest.AutoScaleFont, info + ".AutoScaleFont");
            AssertHelper.AreEqual(areaSrc.BackgroundMode, areaDest.BackgroundMode, info + ".BackgroundMode");
            //==============compare properties============//
            

            //==============compare other===============//
            AssertHelper.AreEqual(areaSrc.Height, areaDest.Height, info + ".Height");
            AssertHelper.AreEqual(areaSrc.Width, areaDest.Width, info + ".Width");
            ShapePropertiesTest.ChartArea_Property_Width(areaSrc.ShapeProperties, areaDest.ShapeProperties, info + ".ShapeProperties");
            AssertHelper.AreEqual(areaSrc.IsAutomaticSize, areaDest.IsAutomaticSize, info + ".IsAutomaticSize");
        }
```

### See Also

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


