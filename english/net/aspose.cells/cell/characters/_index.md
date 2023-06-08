---
title: Cell.Characters
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Returns a Characters object that represents a range of characters within the cell text
type: docs
url: /net/aspose.cells/cell/characters/
---
## Cell.Characters method

Returns a Characters object that represents a range of characters within the cell text.

```csharp
public FontSetting Characters(int startIndex, int length)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | Int32 | The index of the start of the character. |
| length | Int32 | The number of characters. |

### Return Value

Characters object.

### Remarks

This method only works on cell with string value.

### Examples

```csharp
[C#]
Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;
cells["A1"].PutValue("Helloworld");
cells["A1"].Characters(5, 5).Font.IsBold = true;
cells["A1"].Characters(5, 5).Font.Color = Color.Blue;

[Visual Basic]
Dim excel as Workbook = new Workbook()
Dim cells as Cells = exce.Worksheets(0).Cells
cells("A1").PutValue("Helloworld")
cells("A1").Characters(5, 5).Font.IsBold = True
cells("A1").Characters(5, 5).Font.Color = Color.Blue
```

### See Also

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


