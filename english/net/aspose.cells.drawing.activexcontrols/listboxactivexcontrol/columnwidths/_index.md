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
            listBox.Value = &quot;Item1&quot;;
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
            listBox.LinkedCell = &quot;A1&quot;;
            listBox.ListFillRange = &quot;A2:A5&quot;;

            // Add some sample data to the worksheet for the ListBox
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;Item1&quot;);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;Item2&quot;);
            worksheet.Cells[&quot;A4&quot;].PutValue(&quot;Item3&quot;);
            worksheet.Cells[&quot;A5&quot;].PutValue(&quot;Item4&quot;);

            // Save the workbook
            workbook.Save(&quot;ListBoxActiveXControlDemo.xlsx&quot;);

            // Output the results
            Console.WriteLine(&quot;ListBox ActiveX Control created and configured successfully.&quot;);
        }
```

### See Also

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


