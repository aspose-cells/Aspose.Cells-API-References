---
title: FillFormat.GradientDegree
second_title: Aspose.Cells for .NET API Reference
description: FillFormat property. Returns the gradient degree for the specified fill. Only applies for Excel 2007
type: docs
url: /net/aspose.cells.drawing/fillformat/gradientdegree/
---
## FillFormat.GradientDegree property

Returns the gradient degree for the specified fill. Only applies for Excel 2007.

```csharp
public double GradientDegree { get; }
```

### Remarks

Can only be a value from 0.0 (dark) through 1.0 (light).

### Examples

```csharp
// Called: AssertHelper.AreEqual(fillformatSrc.GradientDegree, fillformatDest.GradientDegree, 0.01, info + ".GradientDegree");
public static void Property_GradientDegree(FillFormat fillformatSrc, FillFormat fillformatDest, string info)
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
                    AssertHelper.Property_GradientDegree(fillformatSrc.ImageData, fillformatDest.ImageData, info + ".ImageData");                   
                    break;
            }
            AssertHelper.Property_GradientDegree(fillformatSrc.GradientColor1, fillformatDest.GradientColor1, info + ".GradientColor1");
            AssertHelper.Property_GradientDegree(fillformatSrc.GradientColor2, fillformatDest.GradientColor2, info + ".GradientColor2");
            AssertHelper.AreEqual(fillformatSrc.GradientColorType, fillformatDest.GradientColorType, info + ".GradientColorType");           
            AssertHelper.AreEqual(fillformatSrc.GradientDegree, fillformatDest.GradientDegree, 0.01, info + ".GradientDegree");
            AssertHelper.AreEqual(fillformatSrc.GradientStyle, fillformatDest.GradientStyle, info + ".GradientStyle");          
            AssertHelper.AreEqual(fillformatSrc.GradientVariant, fillformatDest.GradientVariant, info + ".GradientVariant");
            AssertHelper.AreEqual(fillformatSrc.Pattern, fillformatDest.Pattern, info + ".Pattern");    
            
            
            AssertHelper.AreEqual(fillformatSrc.Scale, fillformatDest.Scale, info + ".Scale");
            
        }
```

### See Also

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


