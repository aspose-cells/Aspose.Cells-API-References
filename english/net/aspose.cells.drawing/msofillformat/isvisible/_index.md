---
title: MsoFillFormat.IsVisible
second_title: Aspose.Cells for .NET API Reference
description: MsoFillFormat property. Indicates whether there is fill
type: docs
url: /net/aspose.cells.drawing/msofillformat/isvisible/
---
## MsoFillFormat.IsVisible property

Indicates whether there is fill.

```csharp
public bool IsVisible { get; set; }
```

### Examples

```csharp
// Called: if (picSrc.FillFormat.IsVisible && picDest.FillFormat.IsVisible)
public static void Property_IsVisible(Picture picSrc, Picture picDest, string info)
        {
            if (AssertHelper.checkNull(picSrc, picDest, info))
            {
                return;
            }           
            AssertHelper.AreEqual(picSrc.AutoShapeType, picDest.AutoShapeType, info + ".AutoShapeType");
            AssertHelper.AreEqual(picSrc.ImageType, picDest.ImageType, info + ".ImageFormat");
            //======================compare colors and lines====================//
            AssertHelper.AreEqual(picSrc.FillFormat.IsVisible, picDest.FillFormat.IsVisible, info + ".FillFormat.IsVisible");
            if (picSrc.FillFormat.IsVisible && picDest.FillFormat.IsVisible)
            {
                AssertHelper.equals(picSrc.FillFormat.ForeColor, picDest.FillFormat.ForeColor, info + ".FillFormat.ForeColor");
                AssertHelper.equals(picSrc.FillFormat.BackColor, picDest.FillFormat.BackColor, info + ".FillFormat.BackColor");
                AssertHelper.AreEqual(picSrc.FillFormat.Transparency, picDest.FillFormat.Transparency, info + ".FillFormat.Transparency");
            }
            AssertHelper.AreEqual(picSrc.LineFormat.IsVisible, picDest.LineFormat.IsVisible, info + ".LineFormat.IsVisible");
            if (picSrc.LineFormat.IsVisible && picDest.LineFormat.IsVisible)
            {
                AssertHelper.equals(picSrc.LineFormat.ForeColor, picDest.LineFormat.ForeColor, info + ".LineFormat.ForeColor");
                AssertHelper.equals(picSrc.LineFormat.BackColor, picDest.LineFormat.BackColor, info + ".LineFormat.BackColor");
                AssertHelper.AreEqual(picSrc.LineFormat.Style, picDest.LineFormat.Style, info + ".LineFormat.Style");
                AssertHelper.AreEqual(picSrc.LineFormat.DashStyle, picDest.LineFormat.DashStyle, info + ".LineFormat.DashStyle");
                AssertHelper.AreEqual(picSrc.LineFormat.Weight, picDest.LineFormat.Weight, info + ".LineFormat.Weight");
            }
            //======================compare size===================//
            AssertHelper.AreEqual(picSrc.HeightCM, picDest.HeightCM, info + ".HeightCM");
            AssertHelper.AreEqual(picSrc.WidthCM, picDest.WidthCM, info + ".WidthCM");
            AssertHelper.AreEqual(picSrc.RotationAngle, picDest.RotationAngle, info + ".RotationAngle");
            AssertHelper.AreEqual(picSrc.HeightScale, picDest.HeightScale, info + ".HeightScale");
            AssertHelper.AreEqual(picSrc.IsLockAspectRatio, picDest.IsLockAspectRatio, info + ".IsLockAspectRatio");
            AssertHelper.AreEqual(picSrc.RelativeToOriginalPictureSize, picDest.RelativeToOriginalPictureSize, info + ".RelativeToOriginalPictureSize");
            //=====================compare picture===================//
            //AssertHelper.AreEqual(picSrc.LeftCM, picDest.LeftCM, info + ".LeftCM");
            //AssertHelper.AreEqual(picSrc.TopCM, picDest.TopCM, info + ".TopCM");
            AssertHelper.AreEqual(picSrc.BorderLineColor.IsEmpty, picDest.BorderLineColor.IsEmpty, info + ".BorderLineColor.IsEmpty");
            if (picSrc.BorderLineColor.IsEmpty == false && picDest.BorderLineColor.IsEmpty == false)
            {
                AssertHelper.AreEqual(picSrc.BorderLineColor.GetBrightness(), picDest.BorderLineColor.GetBrightness(), info + ".BorderLineColor");
                AssertHelper.AreEqual(picSrc.BorderWeight, picDest.BorderWeight, info + ".BorderWeight");
            }
            //=====================compare protection================//
            AssertHelper.AreEqual(picSrc.IsLocked, picDest.IsLocked, info + ".IsLocked");
            //=====================compare properties================//
            AssertHelper.AreEqual(picSrc.Placement, picDest.Placement, info + ".Placement");
            AssertHelper.AreEqual(picSrc.IsPrintable, picDest.IsPrintable, info + ".IsPrintable");
            //=====================compare other======================//
            AssertHelper.AreEqual(picSrc.Data, picDest.Data, info + ".Data");
            HyperlinksTest.equals(picSrc.Hyperlink, picDest.Hyperlink, info + ".Hyperlink");
        }
```

### See Also

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


