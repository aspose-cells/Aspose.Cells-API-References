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
// Called: if (picSrc.FillFormat.IsVisible &amp;amp;&amp;amp; picDest.FillFormat.IsVisible)
public static void Property_IsVisible(Picture picSrc, Picture picDest, string info)
        {
            if (AssertHelper.checkNull(picSrc, picDest, info))
            {
                return;
            }           
            AssertHelper.AreEqual(picSrc.AutoShapeType, picDest.AutoShapeType, info + &quot;.AutoShapeType&quot;);
            AssertHelper.AreEqual(picSrc.ImageType, picDest.ImageType, info + &quot;.ImageFormat&quot;);
            //======================compare colors and lines====================//
            AssertHelper.AreEqual(picSrc.FillFormat.IsVisible, picDest.FillFormat.IsVisible, info + &quot;.FillFormat.IsVisible&quot;);
            if (picSrc.FillFormat.IsVisible &amp;&amp; picDest.FillFormat.IsVisible)
            {
                AssertHelper.equals(picSrc.FillFormat.ForeColor, picDest.FillFormat.ForeColor, info + &quot;.FillFormat.ForeColor&quot;);
                AssertHelper.equals(picSrc.FillFormat.BackColor, picDest.FillFormat.BackColor, info + &quot;.FillFormat.BackColor&quot;);
                AssertHelper.AreEqual(picSrc.FillFormat.Transparency, picDest.FillFormat.Transparency, info + &quot;.FillFormat.Transparency&quot;);
            }
            AssertHelper.AreEqual(picSrc.LineFormat.IsVisible, picDest.LineFormat.IsVisible, info + &quot;.LineFormat.IsVisible&quot;);
            if (picSrc.LineFormat.IsVisible &amp;&amp; picDest.LineFormat.IsVisible)
            {
                AssertHelper.equals(picSrc.LineFormat.ForeColor, picDest.LineFormat.ForeColor, info + &quot;.LineFormat.ForeColor&quot;);
                AssertHelper.equals(picSrc.LineFormat.BackColor, picDest.LineFormat.BackColor, info + &quot;.LineFormat.BackColor&quot;);
                AssertHelper.AreEqual(picSrc.LineFormat.Style, picDest.LineFormat.Style, info + &quot;.LineFormat.Style&quot;);
                AssertHelper.AreEqual(picSrc.LineFormat.DashStyle, picDest.LineFormat.DashStyle, info + &quot;.LineFormat.DashStyle&quot;);
                AssertHelper.AreEqual(picSrc.LineFormat.Weight, picDest.LineFormat.Weight, info + &quot;.LineFormat.Weight&quot;);
            }
            //======================compare size===================//
            AssertHelper.AreEqual(picSrc.HeightCM, picDest.HeightCM, info + &quot;.HeightCM&quot;);
            AssertHelper.AreEqual(picSrc.WidthCM, picDest.WidthCM, info + &quot;.WidthCM&quot;);
            AssertHelper.AreEqual(picSrc.RotationAngle, picDest.RotationAngle, info + &quot;.RotationAngle&quot;);
            AssertHelper.AreEqual(picSrc.HeightScale, picDest.HeightScale, info + &quot;.HeightScale&quot;);
            AssertHelper.AreEqual(picSrc.IsLockAspectRatio, picDest.IsLockAspectRatio, info + &quot;.IsLockAspectRatio&quot;);
            AssertHelper.AreEqual(picSrc.RelativeToOriginalPictureSize, picDest.RelativeToOriginalPictureSize, info + &quot;.RelativeToOriginalPictureSize&quot;);
            //=====================compare picture===================//
            //AssertHelper.AreEqual(picSrc.LeftCM, picDest.LeftCM, info + &quot;.LeftCM&quot;);
            //AssertHelper.AreEqual(picSrc.TopCM, picDest.TopCM, info + &quot;.TopCM&quot;);
            AssertHelper.AreEqual(picSrc.BorderLineColor.IsEmpty, picDest.BorderLineColor.IsEmpty, info + &quot;.BorderLineColor.IsEmpty&quot;);
            if (picSrc.BorderLineColor.IsEmpty == false &amp;&amp; picDest.BorderLineColor.IsEmpty == false)
            {
                AssertHelper.AreEqual(picSrc.BorderLineColor.GetBrightness(), picDest.BorderLineColor.GetBrightness(), info + &quot;.BorderLineColor&quot;);
                AssertHelper.AreEqual(picSrc.BorderWeight, picDest.BorderWeight, info + &quot;.BorderWeight&quot;);
            }
            //=====================compare protection================//
            AssertHelper.AreEqual(picSrc.IsLocked, picDest.IsLocked, info + &quot;.IsLocked&quot;);
            //=====================compare properties================//
            AssertHelper.AreEqual(picSrc.Placement, picDest.Placement, info + &quot;.Placement&quot;);
            AssertHelper.AreEqual(picSrc.IsPrintable, picDest.IsPrintable, info + &quot;.IsPrintable&quot;);
            //=====================compare other======================//
            AssertHelper.AreEqual(picSrc.Data, picDest.Data, info + &quot;.Data&quot;);
            HyperlinksTest.equals(picSrc.Hyperlink, picDest.Hyperlink, info + &quot;.Hyperlink&quot;);
        }
```

### See Also

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


