---
title: Enum ShapePathPointValueType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.ShapePathPointValueType enum. Specifies the value type of ShapePathPoint object
type: docs
url: /net/aspose.cells.drawing/shapepathpointvaluetype/
---
## ShapePathPointValueType enumeration

Specifies the value type of [`ShapePathPoint`](../shapepathpoint/) object

```csharp
public enum ShapePathPointValueType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Position | `0` | Specifies the type of the object is location coordinates. The [`ShapePathPoint`](../shapepathpoint/) object stores the coordinate values of a point. |
| Angle | `1` | Specifies the type of the object is angle markers. The [`ShapePathPoint`](../shapepathpoint/) object stores the start and end angles of the arc. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapePathPointValueTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Demonstrate the ShapePathPointValueType enum values
                ShapePathPointValueType positionType = ShapePathPointValueType.Position;
                ShapePathPointValueType angleType = ShapePathPointValueType.Angle;

                // Display the enum values
                Console.WriteLine($"Position type value: {(int)positionType}");
                Console.WriteLine($"Angle type value: {(int)angleType}");

                // Verify the enum values match the expected constants
                Console.WriteLine($"Position equals 0: {positionType == ShapePathPointValueType.Position}");
                Console.WriteLine($"Angle equals 1: {angleType == ShapePathPointValueType.Angle}");

                Console.WriteLine("ShapePathPointValueType enum demonstrated successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ShapePathPointValueType: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


