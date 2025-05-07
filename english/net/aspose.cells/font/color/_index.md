---
title: Font.Color
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets or sets the Color of the font
type: docs
url: /net/aspose.cells/font/color/
---
## Font.Color property

Gets or sets the Color of the font.

```csharp
public Color Color { get; set; }
```

### Examples

```csharp
// Called: style.Font.Color = Color.Yellow;
private void Property_Color(Workbook excel)
		{
            Style style = excel.CreateStyle();
			style.Number = 7;
			style.Name = "Sales";

            style = excel.CreateStyle();
			style.Font.Size = 14;
			style.Font.IsBold = true;
			style.Font.IsItalic = true;
			style.Font.Color = Color.Yellow;
			style.ForegroundColor = Color.Blue;
			style.Pattern = BackgroundType.Solid;
			style.Name = "Header";
		}
```

### See Also

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


