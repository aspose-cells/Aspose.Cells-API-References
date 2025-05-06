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
// Called: Console.WriteLine($&amp;quot;Rendering Cell: {drawObject.Cell.Name}, Value: {drawObject.Cell.Value}&amp;quot;);
public override void Property_Cell(DrawObject drawObject, float x, float y, float width, float height)
        {
            Console.WriteLine($&quot;Drawing object at X: {x}, Y: {y}, Width: {width}, Height: {height}&quot;);
            Console.WriteLine($&quot;Object Type: {drawObject.Type}&quot;);
            Console.WriteLine($&quot;Sheet Index: {drawObject.SheetIndex}, Current Page: {drawObject.CurrentPage}, Total Pages: {drawObject.TotalPages}&quot;);

            if (drawObject.Cell != null)
            {
                Console.WriteLine($&quot;Rendering Cell: {drawObject.Cell.Name}, Value: {drawObject.Cell.Value}&quot;);
            }

            if (drawObject.Shape != null)
            {
                Console.WriteLine($&quot;Rendering Shape: {drawObject.Shape.Name}&quot;);
            }
        }
```

### See Also

* class [Cell](../../../aspose.cells/cell/)
* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


