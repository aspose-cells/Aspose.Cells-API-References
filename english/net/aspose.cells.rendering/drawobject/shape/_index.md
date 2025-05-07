---
title: DrawObject.Shape
second_title: Aspose.Cells for .NET API Reference
description: DrawObject property. Indicates the Shape object when rendering. All properties of shape can be accessed
type: docs
url: /net/aspose.cells.rendering/drawobject/shape/
---
## DrawObject.Shape property

Indicates the Shape object when rendering. All properties of shape can be accessed.

```csharp
public Shape Shape { get; }
```

### Examples

```csharp
// Called: Console.WriteLine($"Rendering Shape: {drawObject.Shape.Name}");
public override void Property_Shape(DrawObject drawObject, float x, float y, float width, float height)
        {
            Console.WriteLine($"Drawing object at X: {x}, Y: {y}, Width: {width}, Height: {height}");
            Console.WriteLine($"Object Type: {drawObject.Type}");
            Console.WriteLine($"Sheet Index: {drawObject.SheetIndex}, Current Page: {drawObject.CurrentPage}, Total Pages: {drawObject.TotalPages}");

            if (drawObject.Cell != null)
            {
                Console.WriteLine($"Rendering Cell: {drawObject.Cell.Name}, Value: {drawObject.Cell.Value}");
            }

            if (drawObject.Shape != null)
            {
                Console.WriteLine($"Rendering Shape: {drawObject.Shape.Name}");
            }
        }
```

### See Also

* class [Shape](../../../aspose.cells.drawing/shape/)
* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


