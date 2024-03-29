---
title: ShapeCollection.AddOleObject
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Adds an OleObject
type: docs
url: /net/aspose.cells.drawing/shapecollection/addoleobject/
---
## ShapeCollection.AddOleObject method

Adds an OleObject.

```csharp
public OleObject AddOleObject(int upperLeftRow, int top, int upperLeftColumn, int left, int height, 
    int width, byte[] imageData)
```

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 |  |
| top | Int32 |  |
| upperLeftColumn | Int32 |  |
| left | Int32 |  |
| height | Int32 |  |
| width | Int32 |  |
| imageData | Byte[] |  |

### Examples

```csharp

[C#]
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    int len = (int)fs.Length;
    byte[] imageData = new byte[len];
    fs.Read(imageData, 0, len);
    OleObject oleObject = shapes.AddOleObject(4, 0, 5, 0, 300, 500, imageData);
}
```

### See Also

* class [OleObject](../../oleobject/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


