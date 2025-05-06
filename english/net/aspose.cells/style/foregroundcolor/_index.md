---
title: Style.ForegroundColor
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets or sets a styles foreground color
type: docs
url: /net/aspose.cells/style/foregroundcolor/
---
## Style.ForegroundColor property

Gets or sets a style's foreground color.

```csharp
public Color ForegroundColor { get; set; }
```

### Remarks

It means no color setting if Color.Empty is returned.

### Examples

```csharp
// Called: AssertHelper.equals(styleSrc.ForegroundColor, styleDest.ForegroundColor, info + &amp;quot;.ForegroundColor&amp;quot;);
public static void Property_ForegroundColor(Style styleSrc, Style styleDest, string info)
        {
            if (AssertHelper.checkNull(styleSrc, styleDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(styleSrc.Pattern, styleDest.Pattern, info + &quot;.Pattern&quot;);
            AssertHelper.equals(styleSrc.ForegroundColor, styleDest.ForegroundColor, info + &quot;.ForegroundColor&quot;);
            AssertHelper.equals(styleSrc.BackgroundColor, styleDest.BackgroundColor, info + &quot;.BackgroundColor&quot;);
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


