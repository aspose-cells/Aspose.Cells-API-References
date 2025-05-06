---
title: ComboBoxActiveXControl.DropButtonStyle
second_title: Aspose.Cells for .NET API Reference
description: ComboBoxActiveXControl property. Specifies the symbol displayed on the drop button
type: docs
url: /net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/dropbuttonstyle/
---
## ComboBoxActiveXControl.DropButtonStyle property

Specifies the symbol displayed on the drop button

```csharp
public DropButtonStyle DropButtonStyle { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine(&amp;quot;DropButtonStyle set to: &amp;quot; + comboBox.DropButtonStyle);
public static void Property_DropButtonStyle()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a ComboBox ActiveX control to the worksheet
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Set properties for the ComboBox
            comboBox.ListWidth = 100;
            comboBox.ListRows = 5;
            comboBox.ColumnCount = 1;
            comboBox.DropButtonStyle = DropButtonStyle.Arrow; // Set the drop button style to Arrow

            // Add some items to the ComboBox
            comboBox.LinkedCell = &quot;A1&quot;;
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Item 1&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;Item 2&quot;);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;Item 3&quot;);
            worksheet.Cells[&quot;A4&quot;].PutValue(&quot;Item 4&quot;);
            comboBox.ListFillRange = &quot;A1:A4&quot;;

            // Save the workbook
            workbook.Save(&quot;DropButtonStyleExample.xlsx&quot;);
            workbook.Save(&quot;DropButtonStyleExample.pdf&quot;);

            // Output the DropButtonStyle used
            Console.WriteLine(&quot;DropButtonStyle set to: &quot; + comboBox.DropButtonStyle);
        }
```

### See Also

* enum [DropButtonStyle](../../dropbuttonstyle/)
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


