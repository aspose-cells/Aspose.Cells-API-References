---
title: ListBoxActiveXControl.ColumnWidths
second_title: Aspose.Cells for .NET API Reference
description: ListBoxActiveXControl property. Gets and sets the width of the column
type: docs
url: /net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/columnwidths/
---
## ListBoxActiveXControl.ColumnWidths property

Gets and sets the width of the column.

```csharp
public double ColumnWidths { get; set; }
```

### Examples

```csharp
// Called: listBox.ColumnWidths = 50;
public static void Property_ColumnWidths()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a ListBox ActiveX control to the worksheet
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 5, 0, 1, 1, 100, 100);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;

            // Set properties for the ListBox
            listBox.ListWidth = 100;
            listBox.BoundColumn = 1;
            listBox.TextColumn = 1;
            listBox.ColumnCount = 2;
            listBox.MatchEntry = ControlMatchEntryType.Complete;
            listBox.ListStyle = ControlListStyle.Plain;
            listBox.SelectionType = SelectionType.Multi;
            listBox.Value = "Item1";
            listBox.BorderOleColor = 0x000000; // Black color
            listBox.SpecialEffect = ControlSpecialEffectType.Flat;
            listBox.ShowColumnHeads = true;
            listBox.IntegralHeight = true;
            listBox.ColumnWidths = 50;

            // Set additional properties inherited from ActiveXControl
            listBox.IsEnabled = true;
            listBox.IsLocked = false;
            listBox.IsTransparent = false;
            listBox.IsAutoSize = false;
            listBox.IMEMode = InputMethodEditorMode.NoControl;
            listBox.TextAlign = TextAlignmentType.Left;
            listBox.IsVisible = true;
            listBox.Shadow = false;
            listBox.LinkedCell = "A1";
            listBox.ListFillRange = "A2:A5";

            // Add some sample data to the worksheet for the ListBox
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["A4"].PutValue("Item3");
            worksheet.Cells["A5"].PutValue("Item4");

            // Save the workbook
            workbook.Save("ListBoxActiveXControlDemo.xlsx");

            // Output the results
            Console.WriteLine("ListBox ActiveX Control created and configured successfully.");
        }
```

### See Also

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


