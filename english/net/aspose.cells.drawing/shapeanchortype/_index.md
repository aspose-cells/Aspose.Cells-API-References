---
title: Enum ShapeAnchorType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.ShapeAnchorType enum. Represents the anchor type
type: docs
url: /net/aspose.cells.drawing/shapeanchortype/
---
## ShapeAnchorType enumeration

Represents the anchor type.

```csharp
public enum ShapeAnchorType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| TwoCellAnchor | `0` | Represents a two cell anchor placeholder |
| OneCellAnchor | `1` | Represents a one cell anchor placeholder |

### Examples

```csharp
// Called: box.AnchorType = ShapeAnchorType.TwoCellAnchor;
public static void Drawing_Type_ShapeAnchorType()
        {
            // Instantiate a new Workbook.
            Workbook workbook = new Workbook();

            // Add a group box to the first worksheet.
            GroupBox box = workbook.Worksheets[0].Shapes.AddGroupBox(1, 0, 1, 0, 300, 250);

            // Set the caption of the group box.
            box.Text = "Age Groups";
            box.Placement = PlacementType.FreeFloating;

            // Make it 2-D box.
            box.Shadow = false;

            // Set additional properties
            box.Name = "GroupBox1";
            box.AlternativeText = "This is a group box";
            box.Title = "Group Box Title";
            box.ZOrderPosition = 1;
            box.IsHidden = false;
            box.IsLockAspectRatio = true;
            box.RotationAngle = 0;
            box.IsPrintable = true;
            box.AutoShapeType = AutoShapeType.Rectangle;
            box.AnchorType = ShapeAnchorType.TwoCellAnchor;
            box.UpperLeftRow = 1;
            box.UpperLeftColumn = 1;
            box.LowerRightRow = 10;
            box.LowerRightColumn = 5;
            box.Width = 300;
            box.Height = 250;
            box.Left = 50;
            box.Top = 50;
            box.Text = "Group Box Text";
            box.HtmlText = "<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>";
            box.TextVerticalOverflow = TextOverflowType.Clip;
            box.TextHorizontalOverflow = TextOverflowType.Clip;
            box.IsTextWrapped = true;
            box.TextOrientationType = TextOrientationType.NoRotation;
            box.TextHorizontalAlignment = TextAlignmentType.Center;
            box.TextVerticalAlignment = TextAlignmentType.Center;
            box.TextDirection = TextDirectionType.LeftToRight;

            // Save the workbook
            workbook.Save("GroupBoxExample.xlsx");
            workbook.Save("GroupBoxExample.pdf");
        }
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


