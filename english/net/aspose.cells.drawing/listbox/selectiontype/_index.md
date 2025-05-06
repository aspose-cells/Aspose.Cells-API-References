---
title: ListBox.SelectionType
second_title: Aspose.Cells for .NET API Reference
description: ListBox property. Gets or sets the selection mode of the specified list box
type: docs
url: /net/aspose.cells.drawing/listbox/selectiontype/
---
## ListBox.SelectionType property

Gets or sets the selection mode of the specified list box.

```csharp
public SelectionType SelectionType { get; set; }
```

### Examples

```csharp
// Called: listBox.SelectionType = SelectionType.Single;
public static void Property_SelectionType()
        {
            // Create a new Workbook.
            Workbook workbook = new Workbook();

            // Get the first worksheet.
            Worksheet sheet = workbook.Worksheets[0];

            // Get the worksheet cells collection.
            Cells cells = sheet.Cells;

            // Input a value.
            cells[&quot;B3&quot;].PutValue(&quot;Choose Dept:&quot;);

            // Set it bold.
            Style style = cells[&quot;B3&quot;].GetStyle();
            style.Font.IsBold = true;
            cells[&quot;B3&quot;].SetStyle(style);

            // Input some values that denote the input range for the list box.
            cells[&quot;A2&quot;].PutValue(&quot;Sales&quot;);
            cells[&quot;A3&quot;].PutValue(&quot;Finance&quot;);
            cells[&quot;A4&quot;].PutValue(&quot;MIS&quot;);
            cells[&quot;A5&quot;].PutValue(&quot;R&amp;D&quot;);
            cells[&quot;A6&quot;].PutValue(&quot;Marketing&quot;);
            cells[&quot;A7&quot;].PutValue(&quot;HRA&quot;);

            // Add a new list box.
            ListBox listBox = sheet.Shapes.AddListBox(2, 0, 3, 0, 122, 100);

            // Set the placement type.
            listBox.Placement = PlacementType.FreeFloating;

            // Set the linked cell.
            listBox.LinkedCell = &quot;A1&quot;;

            // Set the input range.
            listBox.InputRange = &quot;A2:A7&quot;;

            // Set the selection style.
            listBox.SelectionType = SelectionType.Single;

            // Set the list box with 3-D shading.
            listBox.Shadow = true;

            // Set additional properties
            listBox.SelectedIndex = 2; // Select &quot;MIS&quot;
            listBox.MacroName = &quot;DoWork()&quot;;
            listBox.ZOrderPosition = 3;
            listBox.Name = &quot;ListBox1&quot;;
            listBox.AlternativeText = &quot;Department Selection ListBox&quot;;
            listBox.Title = &quot;Department List&quot;;
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
            listBox.Text = &quot;Select a department&quot;;
            listBox.HtmlText = &quot;&lt;Font Style=&apos;FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;&apos;&gt;Select a &lt;b&gt;department&lt;/b&gt;.&lt;/Font&gt;&quot;;
            listBox.TextVerticalOverflow = TextOverflowType.Overflow;
            listBox.TextHorizontalOverflow = TextOverflowType.Overflow;
            listBox.IsTextWrapped = true;
            listBox.TextOrientationType = TextOrientationType.TopToBottom;
            listBox.TextHorizontalAlignment = TextAlignmentType.Center;
            listBox.TextVerticalAlignment = TextAlignmentType.Center;
            listBox.TextDirection = TextDirectionType.LeftToRight;

            // Save the file.
            workbook.Save(&quot;ListBoxExample.xlsx&quot;);
        }
```

### See Also

* enum [SelectionType](../../selectiontype/)
* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


