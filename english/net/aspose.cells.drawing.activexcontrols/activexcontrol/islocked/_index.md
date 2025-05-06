---
title: ActiveXControl.IsLocked
second_title: Aspose.Cells for .NET API Reference
description: ActiveXControl property. Indicates whether data in the control is locked for editing
type: docs
url: /net/aspose.cells.drawing.activexcontrols/activexcontrol/islocked/
---
## ActiveXControl.IsLocked property

Indicates whether data in the control is locked for editing.

```csharp
public bool IsLocked { get; set; }
```

### Examples

```csharp
// Called: checkBox.IsLocked = false;
public static void Property_IsLocked()
        {
            // Create a new workbook and access the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a CheckBox ActiveX control to the worksheet
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 5, 0, 5, 0, 100, 20);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Set properties of the CheckBox ActiveX control
            checkBox.Caption = &quot;I agree&quot;;
            checkBox.IsWordWrapped = true;
            checkBox.Alignment = ControlCaptionAlignmentType.Left;
            checkBox.PicturePosition = ControlPicturePositionType.Center;
            checkBox.SpecialEffect = ControlSpecialEffectType.Flat;
            checkBox.Accelerator = &apos;A&apos;;
            checkBox.Value = CheckValueType.Checked;
            checkBox.IsTripleState = false;
            checkBox.IsEnabled = true;
            checkBox.IsLocked = false;
            checkBox.IsTransparent = false;
            checkBox.IsAutoSize = true;
            checkBox.IMEMode = InputMethodEditorMode.NoControl;
            checkBox.TextAlign = TextAlignmentType.Center;
            checkBox.Width = 150;
            checkBox.Height = 30;
            checkBox.MousePointer = ControlMousePointerType.Default;
            checkBox.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Black);
            checkBox.BackOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.White);
            checkBox.IsVisible = true;
            checkBox.Shadow = false;
            checkBox.LinkedCell = &quot;A1&quot;;
            checkBox.ListFillRange = &quot;A2:A5&quot;;

            // Save the workbook
            workbook.Save(&quot;CheckBoxActiveXControlExample.xlsx&quot;);
            workbook.Save(&quot;CheckBoxActiveXControlExample.pdf&quot;);
        }
```

### See Also

* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


