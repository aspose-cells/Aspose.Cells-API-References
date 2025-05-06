---
title: FillFormat.GradientVariant
second_title: Aspose.Cells for .NET API Reference
description: FillFormat property. Returns the gradient variant for the specified fill. Only applies for Excel 2007
type: docs
url: /net/aspose.cells.drawing/fillformat/gradientvariant/
---
## FillFormat.GradientVariant property

Returns the gradient variant for the specified fill. Only applies for Excel 2007.

```csharp
public int GradientVariant { get; }
```

### Remarks

Can only be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2.

### Examples

```csharp
// Called: AssertHelper.AreEqual(formatSrc.GradientVariant, formatDest.GradientVariant, info + &amp;quot;.GradientVariant&amp;quot;);
public static void Property_GradientVariant(FillFormat formatSrc, FillFormat formatDest, string info)
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
                            AssertHelper.Property_GradientVariant(formatSrc.GradientColor1, formatDest.GradientColor1, info + &quot;.GradientColor1&quot;);
                            AssertHelper.AreEqual(formatSrc.GradientDegree, formatDest.GradientDegree, info + &quot;.GradientDegree&quot;);
                            break;
                        case GradientColorType.TwoColors:
                            AssertHelper.Property_GradientVariant(formatSrc.GradientColor1, formatDest.GradientColor1, info + &quot;.GradientColor1&quot;);
                            AssertHelper.Property_GradientVariant(formatSrc.GradientColor2, formatDest.GradientColor2, info + &quot;.GradientColor2&quot;);                          
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

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


