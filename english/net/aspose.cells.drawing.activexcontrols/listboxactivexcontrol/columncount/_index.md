---
title: ListBoxActiveXControl.ColumnCount
second_title: Aspose.Cells for .NET API Reference
description: ListBoxActiveXControl property. Represents the number of columns to display in a ComboBox or ListBox
type: docs
url: /net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/columncount/
---
## ListBoxActiveXControl.ColumnCount property

Represents the number of columns to display in a ComboBox or ListBox.

```csharp
public int ColumnCount { get; set; }
```

### Examples

```csharp
// Called: listBox.ColumnCount = 1;
public static void Property_ColumnCount()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Item&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;Item 1&quot;);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;Item 2&quot;);
            worksheet.Cells[&quot;A4&quot;].PutValue(&quot;Item 3&quot;);

            // Add a ComboBox ActiveX control to the worksheet
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Set properties for the ComboBox
            comboBox.ListWidth = 100;
            comboBox.ListRows = 3;
            comboBox.ColumnCount = 1;
            comboBox.ListStyle = ControlListStyle.Plain; // Set the ListStyle to Plain

            // Add items to the ComboBox
            comboBox.Value = &quot;Item 1&quot;;
            comboBox.BoundColumn = 1;
            comboBox.TextColumn = 1;

            // Add a ListBox ActiveX control to the worksheet
            var shape2 = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 10, 0, 1, 0, 100, 60);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape2.ActiveXControl;

            // Set properties for the ListBox
            listBox.ColumnCount = 1;
            listBox.ListStyle = ControlListStyle.Option; // Set the ListStyle to Option

            // Add items to the ListBox
            listBox.Value = &quot;Item 1&quot;;
            listBox.BoundColumn = 1;
            listBox.TextColumn = 1;

            // Save the workbook
            workbook.Save(&quot;ControlListStyleExample.xlsx&quot;);
            workbook.Save(&quot;ControlListStyleExample.pdf&quot;);

            // Output the results
            Console.WriteLine(&quot;ComboBox ListStyle: &quot; + comboBox.ListStyle);
            Console.WriteLine(&quot;ListBox ListStyle: &quot; + listBox.ListStyle);
        }
```

### See Also

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


