---
title: Style.Name
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets or sets the name of the style
type: docs
url: /net/aspose.cells/style/name/
---
## Style.Name property

Gets or sets the name of the style.

```csharp
public string Name { get; set; }
```

### Examples

```csharp
// Called: style.Name = "Header";
private void Style_Property_Name(Workbook excel)
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

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


