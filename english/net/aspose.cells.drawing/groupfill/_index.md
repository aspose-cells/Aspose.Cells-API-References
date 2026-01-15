---
title: Class GroupFill
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.GroupFill class. Represents this fill format should inherit the fill properties of the group
type: docs
url: /net/aspose.cells.drawing/groupfill/
---
## GroupFill class

Represents this fill format should inherit the fill properties of the group.

```csharp
public class GroupFill : Fill
```

## Methods

| Name | Description |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Inherited from [`Fill`](../fill/).) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Gets the hash code.(Inherited from [`Fill`](../fill/).) |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassGroupFillDemo
    {
        public static void Run()
        {
            // Create a new workbook for the demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // GroupFill does not expose a public parameterless constructor.
                // For demonstration purposes we obtain a reference (null) of the type.
                GroupFill groupFill = null;

                // Show that the variable of type GroupFill exists.
                Console.WriteLine($"GroupFill variable declared. Type: {typeof(GroupFill).FullName}");

                // Save the workbook (even though we didn't modify it, this demonstrates a complete workflow)
                workbook.Save("GroupFillDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with GroupFill: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


