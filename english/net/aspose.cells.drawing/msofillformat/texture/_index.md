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
// Called: AssertHelper.AreEqual(rectSrc.FillFormat.Texture, rectDest.FillFormat.Texture, info + ".FillFormat.Texture");
public static void Property_Texture(RectangleShape rectSrc, RectangleShape rectDest, string info)
        {
            if (AssertHelper.checkNull(rectSrc, rectDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(rectSrc.AutoShapeType, rectDest.AutoShapeType, info + ".AutoShapeType");
            //================properties are supported in excel 2003 format file===============//
            AssertHelper.AreEqual(rectSrc.UpperLeftRow, rectDest.UpperLeftRow, info + ".UpperLeftRow");
            AssertHelper.AreEqual(rectSrc.UpperLeftColumn, rectDest.UpperLeftColumn, info + ".UpperLeftColumn");
            AssertHelper.AreEqual(rectSrc.LowerRightRow, rectDest.LowerRightRow, info + ".LowerRightRow");
            AssertHelper.AreEqual(rectSrc.LowerRightColumn, rectDest.LowerRightColumn, info + ".LowerRightColumn");
            AssertHelper.AreEqual(rectSrc.Text, rectDest.Text, info + ".Text");
            //===font===//
            FontTest.Property_Texture(rectSrc.Font, rectDest.Font, info + ".Font");
            //===alignment===//
            AssertHelper.AreEqual(rectSrc.TextHorizontalAlignment, rectDest.TextHorizontalAlignment, info + ".TextHorizontalAlignment");
            AssertHelper.AreEqual(rectSrc.TextVerticalAlignment, rectDest.TextVerticalAlignment, info + ".TextVerticalAlignment");
            AssertHelper.AreEqual(rectSrc.TextOrientationType, rectDest.TextOrientationType, info + ".TextOrientationType");
            AssertHelper.AreEqual(rectSrc.TextBody.TextAlignment.AutoSize, rectDest.TextBody.TextAlignment.AutoSize, info + ".TextFrame.AutoSize");
            //===colors and lines===//
            MsoFillFormatTest.Property_Texture(rectSrc.FillFormat, rectDest.FillFormat, info + ".FillFormat");
            MsoLineFormatTest.Property_Texture(rectSrc.LineFormat, rectDest.LineFormat, info + ".LineFormat");
            //===size===//
            AssertHelper.AreEqual(rectSrc.HeightCM, rectDest.HeightCM, info + ".HeightCM");
            AssertHelper.AreEqual(rectSrc.WidthCM, rectDest.WidthCM, info + ".WidthCM");
            AssertHelper.AreEqual(rectSrc.RotationAngle, rectDest.RotationAngle, info + ".RotationAngle");
            AssertHelper.AreEqual(rectSrc.HeightScale, rectDest.HeightScale, info + ".HeightScale");
            AssertHelper.AreEqual(rectSrc.WidthScale, rectDest.WidthScale, info + ".WidthScale");
            AssertHelper.AreEqual(rectSrc.IsLockAspectRatio, rectDest.IsLockAspectRatio, info + ".IsLockAspectRatio");
            //===protection===//
            AssertHelper.AreEqual(rectSrc.IsLocked, rectDest.IsLocked, info + ".IsLocked");
            //===properties====//
            AssertHelper.AreEqual(rectSrc.Placement, rectDest.Placement, info + ".Placement");
            AssertHelper.AreEqual(rectSrc.IsPrintable, rectDest.IsPrintable, info + ".IsPrintable");
            //===margins===//
            TextFrameTest.Property_Texture(rectSrc.TextBody.TextAlignment, rectDest.TextBody.TextAlignment, info+".TextFrame");
            //===Web===//
            AssertHelper.AreEqual(rectSrc.AlternativeText, rectDest.AlternativeText, info + ".AlternativeText");
            //===others===//
            AssertHelper.AreEqual(rectSrc.IsHidden, rectDest.IsHidden, info + ".IsHidden");
            AssertHelper.AreEqual(rectSrc.IsGroup, rectDest.IsGroup, info + ".IsGroup");

            CharactersTest.Property_Texture(rectSrc.GetRichFormattings(), rectDest.GetRichFormattings(), info + ".GetCharacters()");
            HyperlinksTest.Property_Texture(rectSrc.Hyperlink, rectDest.Hyperlink, info + ".Hyperlink");

            //=======================these properties are spported in excel 2007 format file========//
            //===size and properties===//
            AssertHelper.AreEqual(rectSrc.IsPrintable, rectDest.IsPrintable, info + ".IsPrintable");
            //===format shape===//
            AssertHelper.AreEqual(rectSrc.FillFormat.Texture, rectDest.FillFormat.Texture, info + ".FillFormat.Texture");
            AssertHelper.Property_Texture(rectSrc.FillFormat.ImageData, rectDest.FillFormat.ImageData, info + ".FillFormat.ImageData");

            CellsColorTest.Property_Texture(rectSrc.FormatPicture.TransparentColor, rectDest.FormatPicture.TransparentColor, info + ".FormatPicture.TransparentColor");
         
        }
```

### See Also

* enum [TextureType](../../texturetype/)
* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


