---
title: LineFormat.Equals
second_title: Aspose.Cells for .NET API Reference
description: LineFormat method. Determines whether this instance has the same value as another specified LineFormat object
type: docs
url: /net/aspose.cells.drawing/lineformat/equals/
---
## LineFormat.Equals method

Determines whether this instance has the same value as another specified [`LineFormat`](../) object.

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The [`LineFormat`](../) object to compare with this instance. |

### Return Value

true if the value of the obj parameter is the same as the value of this instance; otherwise, false. If obj is null, this method returns false.

### Examples

```csharp

[C#]
//You have to make sure that the index value in this line of code exists
LineFormat obj = workbook.Worksheets[0].Shapes[0].Line;
if (lineFmt.Equals(obj))
{
    //do what you want
}

```

### See Also

* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


