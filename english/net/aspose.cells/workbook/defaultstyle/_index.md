---
title: Workbook.DefaultStyle
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Gets or sets the default Style object of the workbook
type: docs
url: /net/aspose.cells/workbook/defaultstyle/
---
## Workbook.DefaultStyle property

Gets or sets the default [`Style`](../../style/) object of the workbook.

```csharp
public Style DefaultStyle { get; set; }
```

### Remarks

The DefaultStyle property is useful to implement a Style for the whole Workbook.

### Examples

The following code creates and instantiates a new Workbook and sets a default [`Style`](../../style/) to it.

```csharp
[C#]
Workbook workbook = new Workbook();
Style defaultStyle = workbook.DefaultStyle;
defaultStyle.Font.Name = "Tahoma";
workbook.DefaultStyle = defaultStyle;

[Visual Basic]
Dim workbook as Workbook = new Workbook()
Dim defaultStyle as Style = workbook.DefaultStyle
defaultStyle.Font.Name = "Tahoma"
workbook.DefaultStyle = defaultStyle
```

### See Also

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


