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
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Item&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;Apple&quot;);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;Banana&quot;);
            worksheet.Cells[&quot;A4&quot;].PutValue(&quot;Cherry&quot;);

            // Add a ComboBox ActiveX control to the worksheet
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Set properties for the ComboBox
            comboBox.ListWidth = 100;
            comboBox.ListRows = 3;
            comboBox.ColumnCount = 1;
            comboBox.MatchEntry = ControlMatchEntryType.Complete; // Set the MatchEntry type to Complete
            comboBox.IsEditable = true;

            // Add items to the ComboBox
            comboBox.Value = &quot;Apple;Banana;Cherry&quot;;

            // Add a ListBox ActiveX control to the worksheet
            var shape2 = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 10, 0, 1, 0, 100, 60);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape2.ActiveXControl;

            // Set properties for the ListBox
            listBox.ListWidth = 100;
            listBox.ColumnCount = 1;
            listBox.MatchEntry = ControlMatchEntryType.FirstLetter; // Set the MatchEntry type to FirstLetter
            listBox.SelectionType = SelectionType.Single;

            // Add items to the ListBox
            listBox.Value = &quot;Apple;Banana;Cherry&quot;;

            // Save the workbook
            workbook.Save(&quot;ControlMatchEntryTypeExample.xlsx&quot;);
            workbook.Save(&quot;ControlMatchEntryTypeExample.pdf&quot;);

            // Output the results
            Console.WriteLine(&quot;ComboBox and ListBox with different MatchEntry types have been created and saved to ControlMatchEntryTypeExample.xlsx&quot;);
        }
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


