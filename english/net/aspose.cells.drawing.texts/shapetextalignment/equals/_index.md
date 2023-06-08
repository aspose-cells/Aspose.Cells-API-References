---
title: ShapeTextAlignment.Equals
second_title: Aspose.Cells for .NET API Reference
description: ShapeTextAlignment method. Determines whether this instance has the same value as another specified ShapeTextAlignment object
type: docs
url: /net/aspose.cells.drawing.texts/shapetextalignment/equals/
---
## ShapeTextAlignment.Equals method

Determines whether this instance has the same value as another specified [`ShapeTextAlignment`](../) object.

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The [`ShapeTextAlignment`](../) object to compare with this instance. |

### Return Value

true if the value of the obj parameter is the same as the value of this instance; otherwise, false. If obj is null, this method returns false.

### Examples

```csharp

[C#]
//You have to make sure that the index value in this line of code exists
Aspose.Cells.Drawing.Texts.ShapeTextAlignment obj = workbook.Worksheets[0].Shapes[0].TextBody.TextAlignment;
if (shapeTextAlignment.Equals(obj))
{
    //do what you want
}
```

### See Also

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


