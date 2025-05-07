---
title: ComboBoxActiveXControl.ShowDropButtonTypeWhen
second_title: Aspose.Cells for .NET API Reference
description: ComboBoxActiveXControl property. Specifies the symbol displayed on the drop button
type: docs
url: /net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/showdropbuttontypewhen/
---
## ComboBoxActiveXControl.ShowDropButtonTypeWhen property

Specifies the symbol displayed on the drop button

```csharp
public ShowDropButtonType ShowDropButtonTypeWhen { get; set; }
```

### Examples

```csharp
// Called: comboBox.ShowDropButtonTypeWhen = ShowDropButtonType.Focus; // Show drop button when the control has focus
public static void Property_ShowDropButtonTypeWhen()
        {
            // Initialize a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a ComboBox ActiveX control to the worksheet
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 1, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Set properties for the ComboBox ActiveX control
            comboBox.ShowDropButtonTypeWhen = ShowDropButtonType.Focus; // Show drop button when the control has focus
            comboBox.ListWidth = 100;
            comboBox.ListRows = 5;
            comboBox.IsEditable = true;

            // Add some items to the ComboBox
            comboBox.LinkedCell = "A1";
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");

            // Save the workbook
            workbook.Save("ShowDropButtonTypeExample.xlsx");

            return;
        }
```

### See Also

* enum [ShowDropButtonType](../../showdropbuttontype/)
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


