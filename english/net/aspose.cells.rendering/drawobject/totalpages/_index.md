---
title: DrawObject.TotalPages
second_title: Aspose.Cells for .NET API Reference
description: DrawObject property. Indicates total pages in current rendering
type: docs
url: /net/aspose.cells.rendering/drawobject/totalpages/
---
## DrawObject.TotalPages property

Indicates total pages in current rendering.

```csharp
public int TotalPages { get; }
```

### Examples

```csharp
// Called: Console.WriteLine($&amp;quot;Sheet Index: {drawObject.SheetIndex}, Current Page: {drawObject.CurrentPage}, Total Pages: {drawObject.TotalPages}&amp;quot;);
public override void Property_TotalPages(DrawObject drawObject, float x, float y, float width, float height)
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

* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


