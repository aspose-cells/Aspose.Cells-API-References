---
title: Class ReflectionEffect
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.ReflectionEffect class. This class specifies a reflection effect
type: docs
url: /net/aspose.cells.drawing/reflectioneffect/
---
## ReflectionEffect class

This class specifies a reflection effect.

```csharp
public class ReflectionEffect
```

## Properties

| Name | Description |
| --- | --- |
| [Blur](../../aspose.cells.drawing/reflectioneffect/blur/) { get; set; } | Gets and sets the blur radius,in unit of points. |
| [Direction](../../aspose.cells.drawing/reflectioneffect/direction/) { get; set; } | Gets and sets the direction of the alpha gradient ramp relative to the shape itself. |
| [Distance](../../aspose.cells.drawing/reflectioneffect/distance/) { get; set; } | Gets and sets how far to distance the shadow,in unit of points. |
| [FadeDirection](../../aspose.cells.drawing/reflectioneffect/fadedirection/) { get; set; } | Gets and sets the direction to offset the reflection. |
| [RotWithShape](../../aspose.cells.drawing/reflectioneffect/rotwithshape/) { get; set; } | Gets and sets if the reflection should rotate with the shape. |
| [Size](../../aspose.cells.drawing/reflectioneffect/size/) { get; set; } | Gets and sets the end position (along the alpha gradient ramp) of the end alpha value,in unit of percentage |
| [Transparency](../../aspose.cells.drawing/reflectioneffect/transparency/) { get; set; } | Gets and sets the degree of the starting reflection transparency as a value from 0.0 (opaque) through 1.0 (clear). |
| [Type](../../aspose.cells.drawing/reflectioneffect/type/) { get; set; } | Gets and sets the preset reflection effect. |

### Examples

```csharp
// Called: ReflectionEffect reflectionEffect = commentShape.Reflection;
public static void Drawing_Type_ReflectionEffect()
        {
            // Source file
            string fileName = "CommentShape_original.xlsx";

            // Instantiating a Workbook object
            Workbook workbook = new Workbook(fileName);

            // Accessing the first worksheet in the Excel file
            Worksheet worksheet = workbook.Worksheets[0];

            // Accessing the shape collection of the worksheet
            ShapeCollection shapes = worksheet.Shapes;

            // Check if a shape is CommentShape
            CommentShape commentShape = null;
            if (shapes[0].MsoDrawingType == MsoDrawingType.Comment)
            {
                // Represents the shape of the comment
                commentShape = (CommentShape)shapes[0];
            }

            // Demonstrating the usage of CommentShape properties
            if (commentShape != null)
            {
                // Accessing the comment object
                Comment comment = commentShape.Comment;
                Console.WriteLine("Comment Author: " + comment.Author);

                // Setting and getting various properties of CommentShape
                commentShape.MacroName = "DoWork()";
                Console.WriteLine("Macro Name: " + commentShape.MacroName);

                if (commentShape.IsEquation)
                {
                    Console.WriteLine("The shape contains only an equation.");
                }

                if (commentShape.IsSmartArt)
                {
                    Console.WriteLine("The shape is a SmartArt object.");
                }

                commentShape.ZOrderPosition = 3;
                Console.WriteLine("Z Order Position: " + commentShape.ZOrderPosition);

                commentShape.Name = "shape1";
                Console.WriteLine("Shape Name: " + commentShape.Name);

                commentShape.AlternativeText = "a rectangle";
                Console.WriteLine("Alternative Text: " + commentShape.AlternativeText);

                commentShape.Title = "title1";
                Console.WriteLine("Title: " + commentShape.Title);

                // Accessing line and fill formats
                MsoLineFormat lineFormat = commentShape.LineFormat;
                MsoFillFormat fillFormat = commentShape.FillFormat;

                // Accessing shadow, reflection, and glow effects
                ShadowEffect shadowEffect = commentShape.ShadowEffect;
                ReflectionEffect reflectionEffect = commentShape.Reflection;
                GlowEffect glowEffect = commentShape.Glow;

                // Setting and getting dimensions and positions
                commentShape.SoftEdges = 0.5d;
                Console.WriteLine("Soft Edges: " + commentShape.SoftEdges);

                commentShape.IsHidden = false;
                Console.WriteLine("Is Hidden: " + commentShape.IsHidden);

                commentShape.IsLockAspectRatio = false;
                Console.WriteLine("Is Lock Aspect Ratio: " + commentShape.IsLockAspectRatio);

                commentShape.RotationAngle = 60;
                Console.WriteLine("Rotation Angle: " + commentShape.RotationAngle);

                // Accessing hyperlink
                Hyperlink hyperlink = commentShape.Hyperlink;

                // Setting and getting position and size properties
                commentShape.UpperLeftRow = 1;
                commentShape.UpperLeftColumn = 1;
                commentShape.LowerRightRow = 10;
                commentShape.LowerRightColumn = 10;
                commentShape.Width = 100;
                commentShape.Height = 50;

                // Saving the workbook
                workbook.Save("CommentShapeExample.xlsx");
                workbook.Save("CommentShapeExample.pdf");
            }
        }
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


