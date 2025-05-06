---
title: CheckBoxActiveXControl.Value
second_title: Aspose.Cells for .NET API Reference
description: CheckBoxActiveXControl property. Indicates if the control is checked or not
type: docs
url: /net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/value/
---
## CheckBoxActiveXControl.Value property

Indicates if the control is checked or not.

```csharp
public CheckValueType Value { get; set; }
```

### Examples

```csharp
// Called: checkBox.Value = CheckValueType.Checked;
public static void Property_Value()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a CheckBox ActiveX control to the worksheet
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 5, 0, 1, 1, 100, 20);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Set properties for the CheckBox
            checkBox.Caption = &quot;Check Me!&quot;;
            checkBox.Alignment = ControlCaptionAlignmentType.Right;
            checkBox.IsWordWrapped = true;
            checkBox.Value = CheckValueType.Checked;

            // Add a RadioButton ActiveX control to the worksheet
            var shape2 = worksheet.Shapes.AddActiveXControl(ControlType.RadioButton, 10, 0, 1, 1, 100, 20);
            RadioButtonActiveXControl radioButton = (RadioButtonActiveXControl)shape2.ActiveXControl;

            // Set properties for the RadioButton
            radioButton.Caption = &quot;Select Me!&quot;;
            radioButton.Alignment = ControlCaptionAlignmentType.Left;
            radioButton.IsWordWrapped = true;

            // Save the workbook
            workbook.Save(&quot;ControlCaptionAlignmentTypeExample.xlsx&quot;);
            workbook.Save(&quot;ControlCaptionAlignmentTypeExample.pdf&quot;);
            // Output the results
            Console.WriteLine(&quot;CheckBox Alignment: &quot; + checkBox.Alignment);
            Console.WriteLine(&quot;RadioButton Alignment: &quot; + radioButton.Alignment);
        }
```

### See Also

* enum [CheckValueType](../../../aspose.cells.drawing/checkvaluetype/)
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


