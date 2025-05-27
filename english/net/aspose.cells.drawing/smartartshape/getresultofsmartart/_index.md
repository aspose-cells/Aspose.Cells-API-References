---
title: SmartArtShape.GetResultOfSmartArt
second_title: Aspose.Cells for .NET API Reference
description: SmartArtShape method. Converting smart art to grouped shapes
type: docs
url: /net/aspose.cells.drawing/smartartshape/getresultofsmartart/
---
## SmartArtShape.GetResultOfSmartArt method

Converting smart art to grouped shapes.

```csharp
public override GroupShape GetResultOfSmartArt()
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SmartArtShapeMethodGetResultOfSmartArtDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a shape (rectangle) that will be converted to SmartArt
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 200, 200, 0, 0);

            // Get the result of SmartArt as a GroupShape
            GroupShape groupShape = shape.GetResultOfSmartArt();
            
            if(groupShape != null)
            {
                // Example: Print confirmation that SmartArt group exists
                Console.WriteLine("SmartArt group exists");
            }
        }
    }
}
```

### See Also

* class [GroupShape](../../groupshape/)
* class [SmartArtShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


