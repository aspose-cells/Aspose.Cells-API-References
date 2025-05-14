---
title: FillFormat.GradientColor2
second_title: Aspose.Cells for .NET API Reference
description: FillFormat property. Returns the gradient color 2 for the specified fill
type: docs
url: /net/aspose.cells.drawing/fillformat/gradientcolor2/
---
## FillFormat.GradientColor2 property

Returns the gradient color 2 for the specified fill.

```csharp
public Color GradientColor2 { get; }
```

### Remarks

Only when the gradient color type is GradientColorType.TwoColors, this property is meaningful.

### Examples

```csharp
// Called: AssertHelper.equals(formatSrc.GradientColor2, formatDest.GradientColor2, info + ".GradientColor2");
public static void FillFormat_Property_GradientColor2(FillFormat formatSrc, FillFormat formatDest, string info)
        {
            if (AssertHelper.checkNull(formatSrc, formatDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(formatSrc.FillType, formatDest.FillType, info + ".SetType");
            switch (formatSrc.FillType)
            {
                case FillType.None:
                    break;
                case FillType.Gradient:
                    AssertHelper.AreEqual(formatSrc.GradientColorType, formatDest.GradientColorType, info + ".GradientColorType");
                    switch (formatSrc.GradientColorType)
                    {
                        case GradientColorType.None:
                            break;
                        case GradientColorType.OneColor:
                            AssertHelper.FillFormat_Property_GradientColor2(formatSrc.GradientColor1, formatDest.GradientColor1, info + ".GradientColor1");
                            AssertHelper.AreEqual(formatSrc.GradientDegree, formatDest.GradientDegree, info + ".GradientDegree");
                            break;
                        case GradientColorType.TwoColors:
                            AssertHelper.FillFormat_Property_GradientColor2(formatSrc.GradientColor1, formatDest.GradientColor1, info + ".GradientColor1");
                            AssertHelper.FillFormat_Property_GradientColor2(formatSrc.GradientColor2, formatDest.GradientColor2, info + ".GradientColor2");                          
                            break;
                        case GradientColorType.PresetColors:
                            AssertHelper.AreEqual(formatSrc.PresetColor, formatDest.PresetColor, info + ".PresetColor");
                            break;
                    }
                    AssertHelper.AreEqual(formatSrc.GradientStyle, formatDest.GradientStyle, info + ".GradientStyle");
                    AssertHelper.AreEqual(formatSrc.GradientVariant, formatDest.GradientVariant, info + ".GradientVariant");
                    break;
                case FillType.Texture:
                    AssertHelper.AreEqual(formatSrc.Texture, formatDest.Texture, info + ".Texture");
                    break;
                case FillType.Pattern:
                    AssertHelper.AreEqual(formatSrc.Pattern, formatDest.Pattern, info + ".Pattern");
                    break;
            }
        }
```

### See Also

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


