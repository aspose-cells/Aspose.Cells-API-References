---
title: ShapeCollection.AddSpinner
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Adds a Spinner to the worksheet
type: docs
url: /net/aspose.cells.drawing/shapecollection/addspinner/
---
## ShapeCollection.AddSpinner method

Adds a Spinner to the worksheet.

```csharp
public Spinner AddSpinner(int upperLeftRow, int top, int upperLeftColumn, int left, int height, 
    int width)
```

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of Spinner from its left row, in unit of pixel. |
| upperLeftColumn | Int32 | Upper left column index. |
| left | Int32 | Represents the horizontal offset of Spinner from its left column, in unit of pixel. |
| height | Int32 | Represents the height of Spinner, in unit of pixel. |
| width | Int32 | Represents the width of Spinner, in unit of pixel. |

### Return Value

A Spinner object.

### Examples

```csharp

[C#]
//add a spinner
Spinner spinner = shapes.AddSpinner(1, 0, 1, 0, 100, 50);
```

### See Also

* class [Spinner](../../spinner/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


