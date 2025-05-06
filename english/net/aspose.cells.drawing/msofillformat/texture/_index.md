---
title: MsoFillFormat.Texture
second_title: Aspose.Cells for .NET API Reference
description: MsoFillFormat property. Gets the texture fill type
type: docs
url: /net/aspose.cells.drawing/msofillformat/texture/
---
## MsoFillFormat.Texture property

Gets the texture fill type.

```csharp
public TextureType Texture { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(arcSrc.FillFormat.Texture, arcDest.FillFormat.Texture, info+&amp;quot;.Texture&amp;quot;);
public static void Property_Texture(ArcShape arcSrc, ArcShape arcDest, string info)
        {
            if (AssertHelper.checkNull(arcSrc, arcDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(arcSrc.UpperLeftRow, arcDest.UpperLeftRow, info + &quot;.UpperLeftRow&quot;);
            AssertHelper.AreEqual(arcSrc.UpperLeftColumn, arcDest.UpperLeftColumn, info + &quot;.UpperLeftColumn&quot;);
            AssertHelper.AreEqual(arcSrc.LowerRightRow, arcDest.LowerRightRow, info + &quot;.LowerRightRow&quot;);
            AssertHelper.AreEqual(arcSrc.LowerRightColumn, arcDest.LowerRightColumn, info + &quot;.LowerRightColumn&quot;);
            //===========get values of  format shape and compare these==========//    
            //Fill option
            AssertHelper.AreEqual(arcSrc.FillFormat.IsVisible, arcDest.FillFormat.IsVisible, info + &quot;.FillFormat.IsVisible&quot;);
            if (arcSrc.FillFormat.IsVisible &amp;&amp; arcDest.FillFormat.IsVisible)
            {
                AssertHelper.Property_Texture(arcSrc.FillFormat.BackColor, arcDest.FillFormat.BackColor, info + &quot;.FillFormat.BackColor&quot;);
                AssertHelper.Property_Texture(arcSrc.FillFormat.ForeColor, arcDest.FillFormat.ForeColor, info + &quot;.FillFormat.ForeColor&quot;);
                AssertHelper.AreEqual(arcSrc.FillFormat.Transparency, arcDest.FillFormat.Transparency, info + &quot;.FillFormat.Transparency&quot;);  
                AssertHelper.Property_Texture(arcSrc.FillFormat.ImageData, arcDest.FillFormat.ImageData, info+&quot;.ImageData&quot;);
                AssertHelper.AreEqual(arcSrc.FillFormat.Texture, arcDest.FillFormat.Texture, info+&quot;.Texture&quot;);
            }
            //Line Color option
            AssertHelper.AreEqual(arcSrc.LineFormat.IsVisible, arcDest.LineFormat.IsVisible, info + &quot;.LineFormat.IsVisible&quot;);
            if (arcSrc.LineFormat.IsVisible &amp;&amp; arcDest.LineFormat.IsVisible)
            {
                AssertHelper.Property_Texture(arcSrc.LineFormat.BackColor, arcDest.LineFormat.BackColor, info + &quot;.LineFormat.BackColor&quot;);
                AssertHelper.Property_Texture(arcSrc.LineFormat.ForeColor, arcDest.LineFormat.ForeColor, info + &quot;.LineFormat.ForeColor&quot;);
                AssertHelper.AreEqual(arcSrc.LineFormat.DashStyle, arcDest.LineFormat.DashStyle, info + &quot;.LineFormat.DashStyle&quot;);
                AssertHelper.AreEqual(arcSrc.LineFormat.Style, arcDest.LineFormat.Style, info + &quot;.LineFormat.Style&quot;);
                AssertHelper.AreEqual(arcSrc.LineFormat.Weight, arcDest.LineFormat.Weight, info + &quot;.LineFormat.Weight&quot;);
                AssertHelper.AreEqual(arcSrc.LineFormat.Transparency, arcDest.LineFormat.Transparency, info+&quot;.Transparency&quot;);
            }
            //Line style option
            AssertHelper.AreEqual(arcSrc.BeginArrowheadStyle, arcDest.BeginArrowheadStyle, info + &quot;.BeginArrowheadStyle&quot;);
            if (arcSrc.BeginArrowheadStyle != MsoArrowheadStyle.None &amp;&amp; arcDest.BeginArrowheadStyle != MsoArrowheadStyle.None)
            {
                AssertHelper.AreEqual(arcSrc.BeginArrowheadLength, arcDest.BeginArrowheadLength, info + &quot;.BeginArrowheadLength&quot;);
                AssertHelper.AreEqual(arcSrc.BeginArrowheadWidth, arcDest.BeginArrowheadWidth, info + &quot;.BeginArrowheadWidth&quot;);
            }
            AssertHelper.AreEqual(arcSrc.EndArrowheadStyle, arcDest.EndArrowheadStyle, info + &quot;.EndArrowheadStyle&quot;);
            if (arcSrc.EndArrowheadStyle != MsoArrowheadStyle.None &amp;&amp; arcDest.EndArrowheadStyle != MsoArrowheadStyle.None)
            {
                AssertHelper.AreEqual(arcSrc.EndArrowheadLength, arcDest.EndArrowheadLength, info + &quot;.EndArrowheadLength&quot;);
                AssertHelper.AreEqual(arcSrc.EndArrowheadWidth, arcDest.EndArrowheadWidth, info + &quot;.EndArrowheadWidth&quot;);
            }
            //Shadow option
            //3-D Format option
            //3-D Rotation option
            //Picture option
            //TextBox option
            AssertHelper.AreEqual(arcSrc.TextVerticalAlignment, arcDest.TextVerticalAlignment, info+&quot;.TextVerticalAlignment&quot;);
            //==============size and properties options================//
            //size option 
            AssertHelper.AreEqual(arcSrc.Height, arcDest.Height, info + &quot;.Height&quot;);
            AssertHelper.AreEqual(arcSrc.Width, arcDest.Width, info + &quot;.Width&quot;);
            AssertHelper.AreEqual(arcSrc.RotationAngle, arcDest.RotationAngle, info + &quot;.RotationAngle&quot;);
            AssertHelper.AreEqual(arcSrc.HeightScale, arcDest.HeightScale, info + &quot;.HeightScale&quot;);
            AssertHelper.AreEqual(arcSrc.WidthScale, arcDest.WidthScale, info + &quot;.WidthScale&quot;);
            AssertHelper.AreEqual(arcSrc.IsLockAspectRatio, arcDest.IsLockAspectRatio, info + &quot;.IsLockAspectRatio&quot;);
            AssertHelper.AreEqual(arcSrc.RelativeToOriginalPictureSize, arcDest.RelativeToOriginalPictureSize, info+&quot;.RelativeToOriginalPictureSize&quot;);
            
            AssertHelper.AreEqual(arcSrc.Left, arcDest.Left, info+&quot;.Left&quot;);
            AssertHelper.AreEqual(arcSrc.Top, arcDest.Top, info+&quot;.Top&quot;);
            //properties option 
            AssertHelper.AreEqual(arcSrc.Placement, arcDest.Placement, info + &quot;.Placement&quot;);
            AssertHelper.AreEqual(arcSrc.IsPrintable, arcDest.IsPrintable, info + &quot;.IsPrintable&quot;);
            AssertHelper.AreEqual(arcSrc.IsLocked, arcDest.IsLocked, info+&quot;.IsLocked&quot;);
            //alt text option
            AssertHelper.AreEqual(arcSrc.AlternativeText, arcDest.AlternativeText, info+&quot;.AlternativeText&quot;);
            //===============compare other==============//
            //===============compare protection===========//
            AssertHelper.AreEqual(arcSrc.IsLocked, arcDest.IsLocked, info + &quot;.IsLocked&quot;);
            HyperlinksTest.Property_Texture(arcSrc.Hyperlink, arcDest.Hyperlink, info + &quot;.Hyperlink&quot;);
            CellsColorTest.Property_Texture(arcSrc.FormatPicture.TransparentColor, arcSrc.FormatPicture.TransparentColor, info + &quot;.TransparentColor&quot;);        

        }
```

### See Also

* enum [TextureType](../../texturetype/)
* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


