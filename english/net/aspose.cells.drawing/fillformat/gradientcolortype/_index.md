---
title: FillFormat.GradientColorType
second_title: Aspose.Cells for .NET API Reference
description: FillFormat property. Returns the gradient color type for the specified fill
type: docs
url: /net/aspose.cells.drawing/fillformat/gradientcolortype/
---
## FillFormat.GradientColorType property

Returns the gradient color type for the specified fill.

```csharp
public GradientColorType GradientColorType { get; }
```

### Examples

```csharp
// Called: switch (formatSrc.GradientColorType)
public static void Property_GradientColorType(FillFormat formatSrc, FillFormat formatDest, string info)
        {
            if (AssertHelper.checkNull(formatSrc, formatDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(formatSrc.FillType, formatDest.FillType, info + &quot;.SetType&quot;);
            switch (formatSrc.FillType)
            {
                case FillType.None:
                    break;
                case FillType.Gradient:
                    AssertHelper.AreEqual(formatSrc.GradientColorType, formatDest.GradientColorType, info + &quot;.GradientColorType&quot;);
                    switch (formatSrc.GradientColorType)
                    {
                        case GradientColorType.None:
                            break;
                        case GradientColorType.OneColor:
                            AssertHelper.Property_GradientColorType(formatSrc.GradientColor1, formatDest.GradientColor1, info + &quot;.GradientColor1&quot;);
                            AssertHelper.AreEqual(formatSrc.GradientDegree, formatDest.GradientDegree, info + &quot;.GradientDegree&quot;);
                            break;
                        case GradientColorType.TwoColors:
                            AssertHelper.Property_GradientColorType(formatSrc.GradientColor1, formatDest.GradientColor1, info + &quot;.GradientColor1&quot;);
                            AssertHelper.Property_GradientColorType(formatSrc.GradientColor2, formatDest.GradientColor2, info + &quot;.GradientColor2&quot;);                          
                            break;
                        case GradientColorType.PresetColors:
                            AssertHelper.AreEqual(formatSrc.PresetColor, formatDest.PresetColor, info + &quot;.PresetColor&quot;);
                            break;
                    }
                    AssertHelper.AreEqual(formatSrc.GradientStyle, formatDest.GradientStyle, info + &quot;.GradientStyle&quot;);
                    AssertHelper.AreEqual(formatSrc.GradientVariant, formatDest.GradientVariant, info + &quot;.GradientVariant&quot;);
                    break;
                case FillType.Texture:
                    AssertHelper.AreEqual(formatSrc.Texture, formatDest.Texture, info + &quot;.Texture&quot;);
                    break;
                case FillType.Pattern:
                    AssertHelper.AreEqual(formatSrc.Pattern, formatDest.Pattern, info + &quot;.Pattern&quot;);
                    break;
            }
        }
```

### See Also

* enum [GradientColorType](../../gradientcolortype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


