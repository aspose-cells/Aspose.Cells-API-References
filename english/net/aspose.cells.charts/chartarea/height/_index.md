---
title: ChartArea.Height
second_title: Aspose.Cells for .NET API Reference
description: ChartArea property. Gets or sets the vertical offset from its lower right corner row in units of 1/4000 of the chart area
type: docs
url: /net/aspose.cells.charts/chartarea/height/
---
## ChartArea.Height property

Gets or sets the vertical offset from its lower right corner row, in units of 1/4000 of the chart area.

```csharp
[Obsolete("Use ChartArea.HeightRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Height { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Please use ChartArea.HeightRatioToChart property, instead. Height = HeightRatioToChart * 4000. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: AssertHelper.AreEqual(areaSrc.Height, areaDest.Height, info + ".Height");
public static void Property_Height(ChartArea areaSrc, ChartArea areaDest, string info)
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
                //AssertHelper.Property_Height(areaSrc.Border.Color, areaDest.Border.Color, info + ".Border.Color");
                //AssertHelper.AreEqual(areaSrc.Border.Weight, areaDest.Border.Weight, info + ".Border.Weight");
                LineTest.Property_Height(areaSrc.Border, areaDest.Border, info+".Border");
            }
            AssertHelper.AreEqual(areaSrc.Shadow, areaDest.Shadow, info + ".Shadow");
            //area
            AreaTest.Property_Height(areaSrc.Area, areaDest.Area, info + ".Area");
            //==============compare font================//
            FontTest.Property_Height(areaSrc.TextFont, areaDest.TextFont, info + ".TextFont");
            AssertHelper.AreEqual(areaSrc.AutoScaleFont, areaDest.AutoScaleFont, info + ".AutoScaleFont");
            AssertHelper.AreEqual(areaSrc.BackgroundMode, areaDest.BackgroundMode, info + ".BackgroundMode");
            //==============compare properties============//
            

            //==============compare other===============//
            AssertHelper.AreEqual(areaSrc.Height, areaDest.Height, info + ".Height");
            AssertHelper.AreEqual(areaSrc.Width, areaDest.Width, info + ".Width");
            ShapePropertiesTest.Property_Height(areaSrc.ShapeProperties, areaDest.ShapeProperties, info + ".ShapeProperties");
            AssertHelper.AreEqual(areaSrc.IsAutomaticSize, areaDest.IsAutomaticSize, info + ".IsAutomaticSize");
        }
```

### See Also

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


