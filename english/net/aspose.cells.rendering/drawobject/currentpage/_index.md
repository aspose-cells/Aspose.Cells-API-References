---
title: DrawObject.CurrentPage
second_title: Aspose.Cells for .NET API Reference
description: DrawObject property. Indicates the page index of DrawObject. Page index is based on zero. One Sheet contains several pages when rendering
type: docs
url: /net/aspose.cells.rendering/drawobject/currentpage/
---
## DrawObject.CurrentPage property

Indicates the page index of DrawObject. Page index is based on zero. One Sheet contains several pages when rendering.

```csharp
public int CurrentPage { get; }
```

### Examples

```csharp
// Called: Console.WriteLine($"Sheet Index: {drawObject.SheetIndex}, Current Page: {drawObject.CurrentPage}, Total Pages: {drawObject.TotalPages}");
public override void DrawObject_Property_CurrentPage(DrawObject drawObject, float x, float y, float width, float height)
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

* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


