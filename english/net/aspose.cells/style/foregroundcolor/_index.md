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
// Called: AssertHelper.equals(Color.Green, style.ForegroundColor, foldName, className, caseName);
private void Style_Property_ForegroundColor(Style style)
        {
            AssertHelper.equals(Color.Red, style.Borders[BorderType.TopBorder].Color, foldName, className, caseName);
            AssertHelper.AreEqual(CellBorderType.Double, style.Borders[BorderType.TopBorder].LineStyle, foldName, className, caseName);
            AssertHelper.equals(Color.Blue, style.Borders[BorderType.LeftBorder].Color, foldName, className, caseName);
            AssertHelper.AreEqual(CellBorderType.Medium, style.Borders[BorderType.LeftBorder].LineStyle, foldName, className, caseName);
            AssertHelper.equals(Color.Green, style.ForegroundColor, foldName, className, caseName);
            AssertHelper.AreEqual(BackgroundType.HorizontalStripe, style.Pattern, foldName, className, caseName);
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


