---
title: ShapeCollection.AddRadioButton
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Adds a RadioButton to the worksheet
type: docs
url: /net/aspose.cells.drawing/shapecollection/addradiobutton/
---
## ShapeCollection.AddRadioButton method

Adds a RadioButton to the worksheet.

```csharp
public RadioButton AddRadioButton(int upperLeftRow, int top, int upperLeftColumn, int left, 
    int height, int width)
```

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of RadioButton from its left row, in unit of pixel. |
| upperLeftColumn | Int32 | Upper left column index. |
| left | Int32 | Represents the horizontal offset of RadioButton from its left column, in unit of pixel. |
| height | Int32 | Represents the height of RadioButton, in unit of pixel. |
| width | Int32 | Represents the width of RadioButton, in unit of pixel. |

### Return Value

A RadioButton object.

### Examples

```csharp

[C#]
//add a radio button
RadioButton radioButton = shapes.AddRadioButton(1, 0, 1, 0, 100, 50);
```

### See Also

* class [RadioButton](../../radiobutton/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


