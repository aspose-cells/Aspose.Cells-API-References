---
title: GradientFill.FillType
second_title: Aspose.Cells for .NET API Reference
description: GradientFill property. Gets the gradient fill type
type: docs
url: /net/aspose.cells.drawing/gradientfill/filltype/
---
## GradientFill.FillType property

Gets the gradient fill type.

```csharp
public GradientFillType FillType { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(fillformatSrc.GradientFill.FillType, fillformatDest.GradientFill.FillType, info + &amp;quot;.GradientFill.FillType&amp;quot;);
public static void Property_FillType(FillFormat fillformatSrc, FillFormat fillformatDest, string info)
        {
            if (AssertHelper.checkNull(fillformatSrc, fillformatDest, info))
            {
                return;
            }

            AssertHelper.AreEqual(fillformatSrc.FillType, fillformatDest.FillType, info + &quot;.SetType&quot;);
            switch (fillformatSrc.FillType)
            {
                case FillType.None:
                    break;
                case FillType.Gradient://Gradient Fill
                    AssertHelper.AreEqual(fillformatSrc.PresetColor, fillformatDest.PresetColor, info + &quot;.PresetColor&quot;);
                    AssertHelper.AreEqual(fillformatSrc.GradientFill.FillType, fillformatDest.GradientFill.FillType, info + &quot;.GradientFill.FillType&quot;);
                    AssertHelper.AreEqual(fillformatSrc.GradientFill.Angle, fillformatDest.GradientFill.Angle, info + &quot;.GradientFill.Angle&quot;);
                    AssertHelper.AreEqual(fillformatSrc.GradientFill.GradientStops, fillformatDest.GradientFill.GradientStops, info + &quot;.GradientFill.GradientStops&quot;);
                    break;
                case FillType.Pattern:
                    break;
                case FillType.Texture:
                    AssertHelper.AreEqual(fillformatSrc.Texture, fillformatDest.Texture, info + &quot;.Texture&quot;);
                    AssertHelper.AreEqual(fillformatSrc.PictureFormatType, fillformatDest.PictureFormatType, info + &quot;.PictureFormatType&quot;);
                    AssertHelper.Property_FillType(fillformatSrc.ImageData, fillformatDest.ImageData, info + &quot;.ImageData&quot;);                   
                    break;
            }
            AssertHelper.Property_FillType(fillformatSrc.GradientColor1, fillformatDest.GradientColor1, info + &quot;.GradientColor1&quot;);
            AssertHelper.Property_FillType(fillformatSrc.GradientColor2, fillformatDest.GradientColor2, info + &quot;.GradientColor2&quot;);
            AssertHelper.AreEqual(fillformatSrc.GradientColorType, fillformatDest.GradientColorType, info + &quot;.GradientColorType&quot;);           
            AssertHelper.AreEqual(fillformatSrc.GradientDegree, fillformatDest.GradientDegree, 0.01, info + &quot;.GradientDegree&quot;);
            AssertHelper.AreEqual(fillformatSrc.GradientStyle, fillformatDest.GradientStyle, info + &quot;.GradientStyle&quot;);          
            AssertHelper.AreEqual(fillformatSrc.GradientVariant, fillformatDest.GradientVariant, info + &quot;.GradientVariant&quot;);
            AssertHelper.AreEqual(fillformatSrc.Pattern, fillformatDest.Pattern, info + &quot;.Pattern&quot;);    
            
            
            AssertHelper.AreEqual(fillformatSrc.Scale, fillformatDest.Scale, info + &quot;.Scale&quot;);
            
        }
```

### See Also

* enum [GradientFillType](../../gradientfilltype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


