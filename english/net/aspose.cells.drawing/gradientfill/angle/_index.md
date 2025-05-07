---
title: GradientFill.Angle
second_title: Aspose.Cells for .NET API Reference
description: GradientFill property. The angle of linear fill
type: docs
url: /net/aspose.cells.drawing/gradientfill/angle/
---
## GradientFill.Angle property

The angle of linear fill.

```csharp
public float Angle { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(fillformatSrc.GradientFill.Angle, fillformatDest.GradientFill.Angle, info + ".GradientFill.Angle");
public static void Property_Angle(FillFormat fillformatSrc, FillFormat fillformatDest, string info)
        {
            if (AssertHelper.checkNull(fillformatSrc, fillformatDest, info))
            {
                return;
            }

            AssertHelper.AreEqual(fillformatSrc.FillType, fillformatDest.FillType, info + ".SetType");
            switch (fillformatSrc.FillType)
            {
                case FillType.None:
                    break;
                case FillType.Gradient://Gradient Fill
                    AssertHelper.AreEqual(fillformatSrc.PresetColor, fillformatDest.PresetColor, info + ".PresetColor");
                    AssertHelper.AreEqual(fillformatSrc.GradientFill.FillType, fillformatDest.GradientFill.FillType, info + ".GradientFill.FillType");
                    AssertHelper.AreEqual(fillformatSrc.GradientFill.Angle, fillformatDest.GradientFill.Angle, info + ".GradientFill.Angle");
                    AssertHelper.AreEqual(fillformatSrc.GradientFill.GradientStops, fillformatDest.GradientFill.GradientStops, info + ".GradientFill.GradientStops");
                    break;
                case FillType.Pattern:
                    break;
                case FillType.Texture:
                    AssertHelper.AreEqual(fillformatSrc.Texture, fillformatDest.Texture, info + ".Texture");
                    AssertHelper.AreEqual(fillformatSrc.PictureFormatType, fillformatDest.PictureFormatType, info + ".PictureFormatType");
                    AssertHelper.Property_Angle(fillformatSrc.ImageData, fillformatDest.ImageData, info + ".ImageData");                   
                    break;
            }
            AssertHelper.Property_Angle(fillformatSrc.GradientColor1, fillformatDest.GradientColor1, info + ".GradientColor1");
            AssertHelper.Property_Angle(fillformatSrc.GradientColor2, fillformatDest.GradientColor2, info + ".GradientColor2");
            AssertHelper.AreEqual(fillformatSrc.GradientColorType, fillformatDest.GradientColorType, info + ".GradientColorType");           
            AssertHelper.AreEqual(fillformatSrc.GradientDegree, fillformatDest.GradientDegree, 0.01, info + ".GradientDegree");
            AssertHelper.AreEqual(fillformatSrc.GradientStyle, fillformatDest.GradientStyle, info + ".GradientStyle");          
            AssertHelper.AreEqual(fillformatSrc.GradientVariant, fillformatDest.GradientVariant, info + ".GradientVariant");
            AssertHelper.AreEqual(fillformatSrc.Pattern, fillformatDest.Pattern, info + ".Pattern");    
            
            
            AssertHelper.AreEqual(fillformatSrc.Scale, fillformatDest.Scale, info + ".Scale");
            
        }
```

### See Also

* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


