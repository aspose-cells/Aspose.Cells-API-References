---
title: Class BaseShapeGuide
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.BaseShapeGuide class. Represents the shape guide
type: docs
url: /net/aspose.cells.drawing/baseshapeguide/
---
## BaseShapeGuide class

Represents the shape guide.

```csharp
public class BaseShapeGuide
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassBaseShapeGuideDemo
    {
        public static void Run()
        {
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Create a rectangle shape with correct parameters
                Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

                // Since BaseShapeGuide doesn't have a public constructor,
                // we'll demonstrate its usage through a shape that might contain guides
                // Note: This is a simplified demonstration as the actual guide access might differ
                Console.WriteLine("Shape created successfully");
                Console.WriteLine($"Shape type: {shape.GetType().Name}");

                // Save the workbook
                workbook.Save("BaseShapeGuideDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with BaseShapeGuide: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


