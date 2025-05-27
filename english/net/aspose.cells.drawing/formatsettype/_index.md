---
title: Enum FormatSetType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.FormatSetType enum. Fill format set type
type: docs
url: /net/aspose.cells.drawing/formatsettype/
---
## FormatSetType enumeration

Fill format set type.

```csharp
public enum FormatSetType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| None | `0` | No Fill format. |
| IsGradientSet | `1` | Gradient fill format. |
| IsTextureSet | `2` | Texture fill format. |
| IsPatternSet | `3` | Pattern fill format. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class DrawingClassFormatSetTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create gradient-filled rectangle
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 10, 0, 10, 100, 200);
            rectangle.Fill.FillType = FillType.Gradient;
            rectangle.Fill.SetTwoColorGradient(Color.DarkBlue, Color.LightBlue, GradientStyleType.Vertical, 0);

            // Create pattern-filled oval
            Shape oval = worksheet.Shapes.AddOval(2, 150, 0, 10, 100, 200);
            oval.Fill.FillType = FillType.Pattern;
            oval.Fill.Pattern = FillPattern.DarkDownwardDiagonal; // Fixed enum value

            // Create texture-filled line
            Shape line = worksheet.Shapes.AddLine(5, 10, 0, 10, 100, 200);
            line.Fill.FillType = FillType.Texture;
            line.Fill.Texture = TextureType.BlueTissuePaper;

            workbook.Save("FormatSetTypeDemo.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


