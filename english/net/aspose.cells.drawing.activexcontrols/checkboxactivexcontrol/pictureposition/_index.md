---
title: CheckBoxActiveXControl.PicturePosition
second_title: Aspose.Cells for .NET API Reference
description: CheckBoxActiveXControl property. Gets and set the location of the controls picture relative to its caption
type: docs
url: /net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/pictureposition/
---
## CheckBoxActiveXControl.PicturePosition property

Gets and set the location of the control's picture relative to its caption.

```csharp
public ControlPicturePositionType PicturePosition { get; set; }
```

### Examples

```csharp
// Called: checkBox.PicturePosition = ControlPicturePositionType.Center;
public static void CheckBoxActiveXControl_Property_PicturePosition()
        {
            // Create a new workbook and access the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a CheckBox ActiveX control to the worksheet
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 5, 0, 5, 0, 100, 20);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Set properties of the CheckBox ActiveX control
            checkBox.Caption = "I agree";
            checkBox.IsWordWrapped = true;
            checkBox.Alignment = ControlCaptionAlignmentType.Left;
            checkBox.PicturePosition = ControlPicturePositionType.Center;
            checkBox.SpecialEffect = ControlSpecialEffectType.Flat;
            checkBox.Accelerator = 'A';
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
            checkBox.LinkedCell = "A1";
            checkBox.ListFillRange = "A2:A5";

            // Save the workbook
            workbook.Save("CheckBoxActiveXControlExample.xlsx");
            workbook.Save("CheckBoxActiveXControlExample.pdf");
        }
```

### See Also

* enum [ControlPicturePositionType](../../controlpicturepositiontype/)
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


