---
title: ChartFrame.AutoScaleFont
second_title: Aspose.Cells for .NET API Reference
description: ChartFrame property. True if the text in the object changes font size when the object size changes. The default value is True
type: docs
url: /net/aspose.cells.charts/chartframe/autoscalefont/
---
## ChartFrame.AutoScaleFont property

True if the text in the object changes font size when the object size changes. The default value is True.

```csharp
public virtual bool AutoScaleFont { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(cframeSrc.AutoScaleFont, cframeDest.AutoScaleFont, info+".AutoScaleFont");
public static void ChartFrame_Property_AutoScaleFont(ChartFrame cframeSrc, ChartFrame cframeDest, string info)
        {
            if (AssertHelper.checkNull(cframeSrc, cframeDest, info))
            {
                return;
            }
            LineTest.ChartFrame_Property_AutoScaleFont(cframeSrc.Border, cframeDest.Border, info + ".Border");
            AreaTest.ChartFrame_Property_AutoScaleFont(cframeSrc.Area, cframeDest.Area, info + ".Area");
            AssertHelper.AreEqual(cframeSrc.AutoScaleFont, cframeDest.AutoScaleFont, info+".AutoScaleFont");
            AssertHelper.AreEqual(cframeSrc.BackgroundMode, cframeDest.BackgroundMode, info + ".BackgroundMode");
            AssertHelper.AreEqual(cframeSrc.Height, cframeDest.Height, info + ".Height");
            AssertHelper.AreEqual(cframeSrc.Shadow, cframeDest.Shadow, info + ".Shadow");
            FontTest.ChartFrame_Property_AutoScaleFont(cframeSrc.Font, cframeDest.Font, info + ".TextFont");
            AssertHelper.AreEqual(cframeSrc.Width, cframeDest.Width, info + ".Width");
            AssertHelper.AreEqual(cframeSrc.X, cframeDest.X, info + ".X");
            AssertHelper.AreEqual(cframeSrc.Y, cframeDest.Y, info + ".Y");

            AssertHelper.AreEqual(cframeSrc.IsAutomaticSize, cframeDest.IsAutomaticSize, info + ".IsAutomaticSize");
            ShapePropertiesTest.ChartFrame_Property_AutoScaleFont(cframeSrc.ShapeProperties, cframeDest.ShapeProperties, info + ".ShapeProperties");
        }
```

### See Also

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


