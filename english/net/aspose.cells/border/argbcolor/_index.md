---
title: Border.ArgbColor
second_title: Aspose.Cells for .NET API Reference
description: Border property. Gets and sets the color with a 32bit ARGB value
type: docs
url: /net/aspose.cells/border/argbcolor/
---
## Border.ArgbColor property

Gets and sets the color with a 32-bit ARGB value.

```csharp
public int ArgbColor { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(source.ArgbColor, dest.ArgbColor);
public static void Property_ArgbColor(Border source, Border dest)
        {
            bool isSourceNull = (source == null);
            bool isDestNull = (dest == null);
            Assert.AreEqual(isSourceNull, isDestNull);

            if (isSourceNull)
            {
                return;
            }
            Assert.AreEqual(source.LineStyle, dest.LineStyle);
            Assert.AreEqual(source.ArgbColor, dest.ArgbColor);
            Assert.AreEqual(source.ThemeColor, dest.ThemeColor);
            Assert.AreEqual(source.Color, dest.Color);
        }
```

### See Also

* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


