---
title: ShapeTextAlignment.NumberOfColumns
second_title: Aspose.Cells for .NET API Reference
description: ShapeTextAlignment property. Gets and sets the number of columns of text in the bounding rectangle
type: docs
url: /net/aspose.cells.drawing.texts/shapetextalignment/numberofcolumns/
---
## ShapeTextAlignment.NumberOfColumns property

Gets and sets the number of columns of text in the bounding rectangle.

```csharp
public int NumberOfColumns { get; set; }
```

### Examples

```csharp
// Called: shapeTextAlignment.NumberOfColumns = 1;
public static void Property_NumberOfColumns()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Adding a rectangle shape to the worksheet
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 50, 100);

            // Accessing the text alignment settings of the shape
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;

            // Setting the text vertical type to Horizontal
            shapeTextAlignment.TextVerticalType = TextVerticalType.Horizontal;

            // Setting other properties for demonstration
            shapeTextAlignment.IsTextWrapped = true;
            shapeTextAlignment.RotateTextWithShape = true;
            shapeTextAlignment.TextVerticalOverflow = TextOverflowType.Clip;
            shapeTextAlignment.TextHorizontalOverflow = TextOverflowType.Clip;
            shapeTextAlignment.RotationAngle = 90;
            shapeTextAlignment.IsLockedText = false;
            shapeTextAlignment.AutoSize = false;
            shapeTextAlignment.TextShapeType = AutoShapeType.TextBox;
            shapeTextAlignment.TopMarginPt = 2.0d;
            shapeTextAlignment.BottomMarginPt = 2.0d;
            shapeTextAlignment.LeftMarginPt = 2.0d;
            shapeTextAlignment.RightMarginPt = 2.0d;
            shapeTextAlignment.IsAutoMargin = true;
            shapeTextAlignment.NumberOfColumns = 1;

            // Saving the workbook
            workbook.Save(&quot;TextVerticalTypeExample.xlsx&quot;);

            return;
        }
```

### See Also

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


