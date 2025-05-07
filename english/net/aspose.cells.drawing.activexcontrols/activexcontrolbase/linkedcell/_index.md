---
title: ActiveXControlBase.LinkedCell
second_title: Aspose.Cells for .NET API Reference
description: ActiveXControlBase property. Gets and sets the linked cell
type: docs
url: /net/aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/
---
## ActiveXControlBase.LinkedCell property

Gets and sets the linked cell.

```csharp
public string LinkedCell { get; set; }
```

### Examples

```csharp
// Called: activeXControl.LinkedCell = "A1";
public static void Property_LinkedCell()
        {
            // Initialize a new workbook.
            Workbook workbook = new Workbook();

            // Add a RadioButton ActiveXControl.
            Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(ControlType.RadioButton, 1, 0, 1, 0, 100, 50);
            RadioButtonActiveXControl activeXControl = (RadioButtonActiveXControl)shape.ActiveXControl;

            // Setting properties
            activeXControl.GroupName = "GroupName123";
            activeXControl.Alignment = ControlCaptionAlignmentType.Left;
            activeXControl.IsWordWrapped = true;
            activeXControl.Caption = "ExampleButton";
            activeXControl.PicturePosition = ControlPicturePositionType.AboveLeft;
            activeXControl.SpecialEffect = ControlSpecialEffectType.Bump;
            activeXControl.Accelerator = '\0';
            activeXControl.Value = CheckValueType.Checked;
            activeXControl.IsTripleState = false;
            activeXControl.IsEnabled = true;
            activeXControl.IsLocked = false;
            activeXControl.IsTransparent = false;
            activeXControl.IsAutoSize = true;
            activeXControl.IMEMode = InputMethodEditorMode.NoControl;
            activeXControl.TextAlign = TextAlignmentType.Center;
            activeXControl.Width = 100;
            activeXControl.Height = 50;
            activeXControl.MousePointer = ControlMousePointerType.Default;
            activeXControl.ForeOleColor = 0x000000; // Black color
            activeXControl.BackOleColor = 0xFFFFFF; // White color
            activeXControl.IsVisible = true;
            activeXControl.Shadow = false;
            activeXControl.LinkedCell = "A1";
            activeXControl.ListFillRange = "A2:A10";

            // Save the workbook
            workbook.Save("RadioButtonActiveXControlExample.xlsx");
        }
```

### See Also

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


