---
title: MsoFillFormat.ImageData
second_title: Aspose.Cells for .NET API Reference
description: MsoFillFormat property. Gets and sets the Texture and Picture fill data
type: docs
url: /net/aspose.cells.drawing/msofillformat/imagedata/
---
## MsoFillFormat.ImageData property

Gets and sets the Texture and Picture fill data.

```csharp
public byte[] ImageData { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.equals(rectSrc.FillFormat.ImageData, rectDest.FillFormat.ImageData, info + &amp;quot;.FillFormat.ImageData&amp;quot;);
public static void Property_ImageData(RectangleShape rectSrc, RectangleShape rectDest, string info)
        {
            if (AssertHelper.checkNull(rectSrc, rectDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(rectSrc.AutoShapeType, rectDest.AutoShapeType, info + &quot;.AutoShapeType&quot;);
            //================properties are supported in excel 2003 format file===============//
            AssertHelper.AreEqual(rectSrc.UpperLeftRow, rectDest.UpperLeftRow, info + &quot;.UpperLeftRow&quot;);
            AssertHelper.AreEqual(rectSrc.UpperLeftColumn, rectDest.UpperLeftColumn, info + &quot;.UpperLeftColumn&quot;);
            AssertHelper.AreEqual(rectSrc.LowerRightRow, rectDest.LowerRightRow, info + &quot;.LowerRightRow&quot;);
            AssertHelper.AreEqual(rectSrc.LowerRightColumn, rectDest.LowerRightColumn, info + &quot;.LowerRightColumn&quot;);
            AssertHelper.AreEqual(rectSrc.Text, rectDest.Text, info + &quot;.Text&quot;);
            //===font===//
            FontTest.Property_ImageData(rectSrc.Font, rectDest.Font, info + &quot;.Font&quot;);
            //===alignment===//
            AssertHelper.AreEqual(rectSrc.TextHorizontalAlignment, rectDest.TextHorizontalAlignment, info + &quot;.TextHorizontalAlignment&quot;);
            AssertHelper.AreEqual(rectSrc.TextVerticalAlignment, rectDest.TextVerticalAlignment, info + &quot;.TextVerticalAlignment&quot;);
            AssertHelper.AreEqual(rectSrc.TextOrientationType, rectDest.TextOrientationType, info + &quot;.TextOrientationType&quot;);
            AssertHelper.AreEqual(rectSrc.TextBody.TextAlignment.AutoSize, rectDest.TextBody.TextAlignment.AutoSize, info + &quot;.TextFrame.AutoSize&quot;);
            //===colors and lines===//
            MsoFillFormatTest.Property_ImageData(rectSrc.FillFormat, rectDest.FillFormat, info + &quot;.FillFormat&quot;);
            MsoLineFormatTest.Property_ImageData(rectSrc.LineFormat, rectDest.LineFormat, info + &quot;.LineFormat&quot;);
            //===size===//
            AssertHelper.AreEqual(rectSrc.HeightCM, rectDest.HeightCM, info + &quot;.HeightCM&quot;);
            AssertHelper.AreEqual(rectSrc.WidthCM, rectDest.WidthCM, info + &quot;.WidthCM&quot;);
            AssertHelper.AreEqual(rectSrc.RotationAngle, rectDest.RotationAngle, info + &quot;.RotationAngle&quot;);
            AssertHelper.AreEqual(rectSrc.HeightScale, rectDest.HeightScale, info + &quot;.HeightScale&quot;);
            AssertHelper.AreEqual(rectSrc.WidthScale, rectDest.WidthScale, info + &quot;.WidthScale&quot;);
            AssertHelper.AreEqual(rectSrc.IsLockAspectRatio, rectDest.IsLockAspectRatio, info + &quot;.IsLockAspectRatio&quot;);
            //===protection===//
            AssertHelper.AreEqual(rectSrc.IsLocked, rectDest.IsLocked, info + &quot;.IsLocked&quot;);
            //===properties====//
            AssertHelper.AreEqual(rectSrc.Placement, rectDest.Placement, info + &quot;.Placement&quot;);
            AssertHelper.AreEqual(rectSrc.IsPrintable, rectDest.IsPrintable, info + &quot;.IsPrintable&quot;);
            //===margins===//
            TextFrameTest.Property_ImageData(rectSrc.TextBody.TextAlignment, rectDest.TextBody.TextAlignment, info+&quot;.TextFrame&quot;);
            //===Web===//
            AssertHelper.AreEqual(rectSrc.AlternativeText, rectDest.AlternativeText, info + &quot;.AlternativeText&quot;);
            //===others===//
            AssertHelper.AreEqual(rectSrc.IsHidden, rectDest.IsHidden, info + &quot;.IsHidden&quot;);
            AssertHelper.AreEqual(rectSrc.IsGroup, rectDest.IsGroup, info + &quot;.IsGroup&quot;);

            CharactersTest.Property_ImageData(rectSrc.GetRichFormattings(), rectDest.GetRichFormattings(), info + &quot;.GetCharacters()&quot;);
            HyperlinksTest.Property_ImageData(rectSrc.Hyperlink, rectDest.Hyperlink, info + &quot;.Hyperlink&quot;);

            //=======================these properties are spported in excel 2007 format file========//
            //===size and properties===//
            AssertHelper.AreEqual(rectSrc.IsPrintable, rectDest.IsPrintable, info + &quot;.IsPrintable&quot;);
            //===format shape===//
            AssertHelper.AreEqual(rectSrc.FillFormat.Texture, rectDest.FillFormat.Texture, info + &quot;.FillFormat.Texture&quot;);
            AssertHelper.Property_ImageData(rectSrc.FillFormat.ImageData, rectDest.FillFormat.ImageData, info + &quot;.FillFormat.ImageData&quot;);

            CellsColorTest.Property_ImageData(rectSrc.FormatPicture.TransparentColor, rectDest.FormatPicture.TransparentColor, info + &quot;.FormatPicture.TransparentColor&quot;);
         
        }
```

### See Also

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


