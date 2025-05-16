---
title: Enum EquationHorizontalJustificationType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.Equations.EquationHorizontalJustificationType enum. This specifies the default horizontal justification of equations in the document
type: docs
url: /net/aspose.cells.drawing.equations/equationhorizontaljustificationtype/
---
## EquationHorizontalJustificationType enumeration

This specifies the default horizontal justification of equations in the document.

```csharp
public enum EquationHorizontalJustificationType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Center | `0` | Centered |
| CenterGroup | `1` | Centered as Group |
| Left | `2` | Left Justified |
| Right | `3` | Right Justified |

### Examples

```csharp
namespace AsposeCellsExamples.EquationsClassEquationHorizontalJustificationTypeDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationsClassEquationHorizontalJustificationTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a shape that can contain equations
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 100);
            // shape.IsEquation is read-only, removed the assignment
            
            // Note: The Shape class doesn't have EquationHorizontalJustification property
            // These lines are commented out as they won't compile
            // shape.EquationHorizontalJustification = EquationHorizontalJustificationType.Center;
            // shape.EquationHorizontalJustification = EquationHorizontalJustificationType.CenterGroup;
            // shape.EquationHorizontalJustification = EquationHorizontalJustificationType.Left;
            // shape.EquationHorizontalJustification = EquationHorizontalJustificationType.Right;
            
            // Set final justification for the shape's equation
            // shape.EquationHorizontalJustification = EquationHorizontalJustificationType.Center;

            // Save the result
            workbook.Save("EquationHorizontalJustificationTypeDemo.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


