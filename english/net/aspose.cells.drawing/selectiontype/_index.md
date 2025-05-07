---
title: Enum SelectionType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.SelectionType enum. The selection type of list box
type: docs
url: /net/aspose.cells.drawing/selectiontype/
---
## SelectionType enumeration

The selection type of list box.

```csharp
public enum SelectionType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Single | `0` | Sigle selection type. |
| Multi | `1` | Multiple selection type. |
| Extend | `2` | Extend selection type. |

### Examples

```csharp
// Called: listBox.SelectionType = SelectionType.Single;
public static void Type_SelectionType()
        {
            // Create a new Workbook.
            Workbook workbook = new Workbook();

            // Get the first worksheet.
            Worksheet sheet = workbook.Worksheets[0];

            // Get the worksheet cells collection.
            Cells cells = sheet.Cells;

            // Input a value.
            cells["B3"].PutValue("Choose Dept:");

            // Set it bold.
            Style style = cells["B3"].GetStyle();
            style.Font.IsBold = true;
            cells["B3"].SetStyle(style);

            // Input some values that denote the input range for the list box.
            cells["A2"].PutValue("Sales");
            cells["A3"].PutValue("Finance");
            cells["A4"].PutValue("MIS");
            cells["A5"].PutValue("R&D");
            cells["A6"].PutValue("Marketing");
            cells["A7"].PutValue("HRA");

            // Add a new list box.
            ListBox listBox = sheet.Shapes.AddListBox(2, 0, 3, 0, 122, 100);

            // Set the placement type.
            listBox.Placement = PlacementType.FreeFloating;

            // Set the linked cell.
            listBox.LinkedCell = "A1";

            // Set the input range.
            listBox.InputRange = "A2:A7";

            // Set the selection style.
            listBox.SelectionType = SelectionType.Single;

            // Set the list box with 3-D shading.
            listBox.Shadow = true;

            // Set additional properties
            listBox.SelectedIndex = 2; // Select "MIS"
            listBox.MacroName = "DoWork()";
            listBox.ZOrderPosition = 3;
            listBox.Name = "ListBox1";
            listBox.AlternativeText = "Department Selection ListBox";
            listBox.Title = "Department List";
            listBox.SoftEdges = 0.5d;
            listBox.IsHidden = false;
            listBox.IsLockAspectRatio = true;
            listBox.RotationAngle = 45;
            listBox.IsPrintable = true;
            listBox.AutoShapeType = AutoShapeType.Rectangle;
            listBox.AnchorType = ShapeAnchorType.TwoCellAnchor;
            listBox.UpperLeftRow = 2;
            listBox.UpperLeftColumn = 1;
            listBox.LowerRightRow = 10;
            listBox.LowerRightColumn = 5;
            listBox.Width = 200;
            listBox.Height = 100;
            listBox.Left = 50;
            listBox.Top = 50;
            listBox.Text = "Select a department";
            listBox.HtmlText = "<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>Select a <b>department</b>.</Font>";
            listBox.TextVerticalOverflow = TextOverflowType.Overflow;
            listBox.TextHorizontalOverflow = TextOverflowType.Overflow;
            listBox.IsTextWrapped = true;
            listBox.TextOrientationType = TextOrientationType.TopToBottom;
            listBox.TextHorizontalAlignment = TextAlignmentType.Center;
            listBox.TextVerticalAlignment = TextAlignmentType.Center;
            listBox.TextDirection = TextDirectionType.LeftToRight;

            // Save the file.
            workbook.Save("ListBoxExample.xlsx");
        }
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


