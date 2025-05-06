---
title: Style.BackgroundColor
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets or sets a styles background color
type: docs
url: /net/aspose.cells/style/backgroundcolor/
---
## Style.BackgroundColor property

Gets or sets a style's background color.

```csharp
public Color BackgroundColor { get; set; }
```

### Remarks

If you want to set a cell's color, please use Style.ForegroundColor property. Only if the cell style pattern is other than none or solid, this property will take effect.

### Examples

```csharp
// Called: style.BackgroundColor = Color.AliceBlue;
private static void Property_BackgroundColor(Cells cell, int rowDataNumber, int maxColumn, string header, string formula)
        {
            // todo: we need to identify the column on which we want to apply the formula by using LINQ.
            Style style = cell[rowDataNumber + 1, maxColumn].GetStyle();
            style.ForegroundColor = Color.AliceBlue;
            style.BackgroundColor = Color.AliceBlue;
            cell[rowDataNumber, 0].Value = header;
            cell[rowDataNumber, maxColumn].Formula = formula;
            cell[rowDataNumber + 1, maxColumn].SetStyle(style);
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


