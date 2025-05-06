---
title: DrawObject.SheetIndex
second_title: Aspose.Cells for .NET API Reference
description: DrawObject property. Indicates current sheet index of DrawObject
type: docs
url: /net/aspose.cells.rendering/drawobject/sheetindex/
---
## DrawObject.SheetIndex property

Indicates current sheet index of DrawObject.

```csharp
public int SheetIndex { get; }
```

### Examples

```csharp
// Called: Console.WriteLine($&amp;quot;Sheet Index: {drawObject.SheetIndex}, Current Page: {drawObject.CurrentPage}, Total Pages: {drawObject.TotalPages}&amp;quot;);
public override void Property_SheetIndex(DrawObject drawObject, float x, float y, float width, float height)
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


