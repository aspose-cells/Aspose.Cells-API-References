---
title: ShapeCollection.AddListBox
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Adds a ListBox to the worksheet
type: docs
url: /net/aspose.cells.drawing/shapecollection/addlistbox/
---
## ShapeCollection.AddListBox method

Adds a ListBox to the worksheet.

```csharp
public ListBox AddListBox(int upperLeftRow, int top, int upperLeftColumn, int left, int height, 
    int width)
```

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of ListBox from its left row, in unit of pixel. |
| upperLeftColumn | Int32 | Upper left column index. |
| left | Int32 | Represents the horizontal offset of ListBox from its left column, in unit of pixel. |
| height | Int32 | Represents the height of ListBox, in unit of pixel. |
| width | Int32 | Represents the width of ListBox, in unit of pixel. |

### Return Value

A ListBox object.

### Examples

```csharp

[C#]
//add a list box
ListBox listBox = shapes.AddListBox(1, 0, 1, 0, 100, 50);
```

### See Also

* class [ListBox](../../listbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


