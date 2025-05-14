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
// Called: comboBox.DropButtonStyle = DropButtonStyle.Arrow; // Set the drop button style to Arrow
public static void ComboBoxActiveXControl_Property_DropButtonStyle()
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
            comboBox.LinkedCell = "A1";
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            comboBox.ListFillRange = "A1:A4";

            // Save the workbook
            workbook.Save("DropButtonStyleExample.xlsx");
            workbook.Save("DropButtonStyleExample.pdf");

            // Output the DropButtonStyle used
            Console.WriteLine("DropButtonStyle set to: " + comboBox.DropButtonStyle);
        }
```

### See Also

* enum [DropButtonStyle](../../dropbuttonstyle/)
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


