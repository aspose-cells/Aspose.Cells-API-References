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
// Called: comboBox.AnchorType = ShapeAnchorType.TwoCellAnchor; // Set the anchor type
public static void Type_ShapeAnchorType()
        {
            // Create a new Workbook.
            Workbook workbook = new Workbook();

            // Get the first worksheet.
            Worksheet sheet = workbook.Worksheets[0];

            // Get the worksheet cells collection.
            Cells cells = sheet.Cells;

            // Input a value.
            cells[&quot;B3&quot;].PutValue(&quot;Employee:&quot;);

            // Set it bold.
            Style style = cells[&quot;B3&quot;].GetStyle();
            style.Font.IsBold = true;
            cells[&quot;B3&quot;].SetStyle(style);

            // Input some values that denote the input range for the combo box.
            cells[&quot;A2&quot;].PutValue(&quot;Emp001&quot;);
            cells[&quot;A3&quot;].PutValue(&quot;Emp002&quot;);
            cells[&quot;A4&quot;].PutValue(&quot;Emp003&quot;);
            cells[&quot;A5&quot;].PutValue(&quot;Emp004&quot;);
            cells[&quot;A6&quot;].PutValue(&quot;Emp005&quot;);
            cells[&quot;A7&quot;].PutValue(&quot;Emp006&quot;);

            // Add a new combo box.
            ComboBox comboBox = sheet.Shapes.AddComboBox(2, 0, 2, 0, 22, 100);

            // Set the linked cell;
            comboBox.LinkedCell = &quot;A1&quot;;

            // Set the input range.
            comboBox.InputRange = &quot;A2:A7&quot;;

            // Set no. of list lines displayed in the combo box&apos;s list portion.
            comboBox.DropDownLines = 5;

            // Set the combo box with 3-D shading.
            comboBox.Shadow = true;

            // Set additional properties
            comboBox.SelectedIndex = 2; // Select the third item (zero-based index)
            comboBox.MacroName = &quot;DoWork()&quot;; // Set the name of macro
            comboBox.ZOrderPosition = 3; // Set the Z-order position
            comboBox.Name = &quot;EmployeeComboBox&quot;; // Set the name of the combo box
            comboBox.AlternativeText = &quot;Select an employee&quot;; // Set alternative text
            comboBox.Title = &quot;Employee Selection&quot;; // Set the title of the combo box
            comboBox.SoftEdges = 0.5d; // Set the radius of blur to apply to the edges
            comboBox.IsHidden = false; // Ensure the combo box is visible
            comboBox.IsLockAspectRatio = true; // Lock the aspect ratio of the combo box
            comboBox.RotationAngle = 0; // Set the rotation angle of the combo box
            comboBox.IsPrintable = true; // Ensure the combo box is printable
            comboBox.AutoShapeType = AutoShapeType.Rectangle; // Set the auto shape type
            comboBox.AnchorType = ShapeAnchorType.TwoCellAnchor; // Set the anchor type
            comboBox.Placement = PlacementType.MoveAndSize; // Set the placement type
            comboBox.UpperLeftRow = 2; // Set the upper left row
            comboBox.UpperLeftColumn = 0; // Set the upper left column
            comboBox.LowerRightRow = 22; // Set the lower right row
            comboBox.LowerRightColumn = 100; // Set the lower right column
            comboBox.Width = 100; // Set the width of the combo box
            comboBox.Height = 22; // Set the height of the combo box
            comboBox.Left = 0; // Set the left position
            comboBox.Top = 2; // Set the top position
            comboBox.WidthScale = 100; // Set the width scale
            comboBox.HeightScale = 100; // Set the height scale
            comboBox.Text = &quot;Select an employee&quot;; // Set the text of the combo box
            comboBox.HtmlText = &quot;&lt;Font Style=&apos;FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;&apos;&gt;Select an employee&lt;/Font&gt;&quot;; // Set the HTML text
            comboBox.TextVerticalOverflow = TextOverflowType.Overflow; // Set the text vertical overflow type
            comboBox.TextHorizontalOverflow = TextOverflowType.Overflow; // Set the text horizontal overflow type
            comboBox.IsTextWrapped = true; // Set the text wrapped type
            comboBox.TextOrientationType = TextOrientationType.TopToBottom; // Set the text orientation type
            comboBox.TextHorizontalAlignment = TextAlignmentType.Center; // Set the text horizontal alignment type
            comboBox.TextVerticalAlignment = TextAlignmentType.Center; // Set the text vertical alignment type
            comboBox.TextDirection = TextDirectionType.LeftToRight; // Set the text direction

            // AutoFit Columns
            sheet.AutoFitColumns();

            // Saves the file.
            workbook.Save(&quot;ComboBoxExample.xlsx&quot;);
            workbook.Save(&quot;ComboBoxExample.pdf&quot;);
        }
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


