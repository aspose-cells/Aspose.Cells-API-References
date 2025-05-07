---
title: MsoLineFormat.BackColor
second_title: Aspose.Cells for .NET API Reference
description: MsoLineFormat property. Gets and sets the border line back color
type: docs
url: /net/aspose.cells.drawing/msolineformat/backcolor/
---
## MsoLineFormat.BackColor property

Gets and sets the border line back color.

```csharp
public Color BackColor { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(groupSrc.LineFormat.BackColor, groupDest.LineFormat.BackColor, info + ".LineFormat.BackColor");
public static void Property_BackColor(GroupShape groupSrc, GroupShape groupDest, string info)
        {
            
            if (AssertHelper.checkNull(groupSrc, groupDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(groupSrc.UpperLeftRow, groupDest.UpperLeftRow, info + ".UpperLeftRow");
            AssertHelper.AreEqual(groupSrc.UpperLeftColumn, groupDest.UpperLeftColumn, info + ".UpperLeftColumn");
            AssertHelper.AreEqual(groupSrc.LowerRightRow, groupDest.LowerRightRow, info + ".LowerRightRow");
            AssertHelper.AreEqual(groupSrc.LowerRightColumn, groupDest.LowerRightColumn, info + ".LowerRightColumn");   
            //==================compare colors and lines===============//
            AssertHelper.AreEqual(groupSrc.FillFormat.IsVisible, groupDest.FillFormat.IsVisible, info + ".FillFormat.IsVisible");
            if (groupSrc.FillFormat.IsVisible && groupDest.FillFormat.IsVisible)
            {
                AssertHelper.Property_BackColor(groupSrc.FillFormat.ForeColor, groupDest.FillFormat.ForeColor, info + ".FillFormat.ForeColor");
                AssertHelper.Property_BackColor(groupSrc.FillFormat.BackColor, groupDest.FillFormat.BackColor, info + ".FillFormat.BackColor");
                AssertHelper.AreEqual(groupSrc.FillFormat.Transparency, groupDest.FillFormat.Transparency, info + ".FillFormat.Transparency");
            }
            AssertHelper.AreEqual(groupSrc.LineFormat.IsVisible, groupDest.LineFormat.IsVisible, info + ".LineFormat.IsVisible");
            if (groupSrc.LineFormat.IsVisible && groupDest.LineFormat.IsVisible)
            {
                AssertHelper.Property_BackColor(groupSrc.LineFormat.ForeColor, groupDest.LineFormat.ForeColor, info + ".LineFormat.ForeColor");
                AssertHelper.AreEqual(groupSrc.LineFormat.BackColor, groupDest.LineFormat.BackColor, info + ".LineFormat.BackColor");
                AssertHelper.AreEqual(groupSrc.LineFormat.Style, groupDest.LineFormat.Style, info + ".LineFormat.Style");
                AssertHelper.AreEqual(groupSrc.LineFormat.DashStyle, groupDest.LineFormat.DashStyle, info + ".LineFormat.DashStyle");
                AssertHelper.AreEqual(groupSrc.LineFormat.Weight, groupDest.LineFormat.Weight, info + ".LineFormat.Weight");
            }
            //======================compare size=====================//
            AssertHelper.AreEqual(groupSrc.HeightCM, groupDest.HeightCM, info + ".HeightCM");
            AssertHelper.AreEqual(groupSrc.WidthCM, groupDest.WidthCM, info + ".WidthCM");
            AssertHelper.AreEqual(groupSrc.RotationAngle, groupDest.RotationAngle, info + ".RotationAngle");
            AssertHelper.AreEqual(groupSrc.HeightScale, groupDest.HeightScale, info + ".HeightScale");
            AssertHelper.AreEqual(groupSrc.WidthScale, groupDest.WidthScale, info + ".WidthScale");
            AssertHelper.AreEqual(groupSrc.IsLockAspectRatio, groupDest.IsLockAspectRatio, info + ".IsLockAspectRatio");
            //======================compare protection================//
            AssertHelper.AreEqual(groupSrc.IsLocked, groupDest.IsLocked, info + ".IsLocked");
            //======================compare properties================//
            AssertHelper.AreEqual(groupSrc.Placement, groupDest.Placement, info + ".Placement");
            AssertHelper.AreEqual(groupSrc.IsPrintable, groupDest.IsPrintable, info + ".IsPrintable");
        }
```

### See Also

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


