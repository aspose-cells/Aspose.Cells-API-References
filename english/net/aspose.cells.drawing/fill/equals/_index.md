---
title: Fill.Equals
second_title: Aspose.Cells for .NET API Reference
description: Fill method. /
type: docs
url: /net/aspose.cells.drawing/fill/equals/
---
## Fill.Equals method

/

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object |  |

### Examples

```csharp
namespace AsposeCellsExamples.FillMethodEqualsWithObjectDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class FillMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create two rectangle shapes with identical dimensions
            Shape shape1 = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 50, 50);
            Shape shape2 = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 50, 50);

            // Get fill formats from both shapes
            FillFormat fill1 = shape1.Fill;
            FillFormat fill2 = shape2.Fill;

            try
            {
                // Compare fill objects using Equals(Object)
                bool areEqual = fill1.Equals((object)fill2);

                Console.WriteLine($"Fill objects equality check result: {areEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            workbook.Save("FillMethodEqualsWithObjectDemo.xlsx");
        }
    }
}
```

### See Also

* class [Fill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


