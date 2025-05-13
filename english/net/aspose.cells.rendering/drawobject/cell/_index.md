---
title: DrawObject.Cell
second_title: Aspose.Cells for .NET API Reference
description: DrawObject property. Indicates the Cell object when rendering. All properties of cell can be accessed
type: docs
url: /net/aspose.cells.rendering/drawobject/cell/
---
## DrawObject.Cell property

Indicates the Cell object when rendering. All properties of cell can be accessed.

```csharp
public Cell Cell { get; }
```

### Examples

```csharp
// Called: if (drawObject.Cell != null)
public override void DrawObject_Property_Cell(DrawObject drawObject, float x, float y, float width, float height)
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

* class [Cell](../../../aspose.cells/cell/)
* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


