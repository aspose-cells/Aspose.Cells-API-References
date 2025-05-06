---
title: ActiveXControlBase.Shadow
second_title: Aspose.Cells for .NET API Reference
description: ActiveXControlBase property. Indicates whether to show a shadow
type: docs
url: /net/aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/
---
## ActiveXControlBase.Shadow property

Indicates whether to show a shadow.

```csharp
public virtual bool Shadow { get; set; }
```

### Examples

```csharp
// Called: activeXControl.Shadow = false;
public static void Property_Shadow()
        {
            // Initialize a new workbook.
            Workbook workbook = new Workbook();

            // Add a RadioButton ActiveXControl.
            Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(ControlType.RadioButton, 1, 0, 1, 0, 100, 50);
            RadioButtonActiveXControl activeXControl = (RadioButtonActiveXControl)shape.ActiveXControl;

            // Setting properties
            activeXControl.GroupName = &quot;GroupName123&quot;;
            activeXControl.Alignment = ControlCaptionAlignmentType.Left;
            activeXControl.IsWordWrapped = true;
            activeXControl.Caption = &quot;ExampleButton&quot;;
            activeXControl.PicturePosition = ControlPicturePositionType.AboveLeft;
            activeXControl.SpecialEffect = ControlSpecialEffectType.Bump;
            activeXControl.Accelerator = &apos;\0&apos;;
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
            activeXControl.LinkedCell = &quot;A1&quot;;
            activeXControl.ListFillRange = &quot;A2:A10&quot;;

            // Save the workbook
            workbook.Save(&quot;RadioButtonActiveXControlExample.xlsx&quot;);
        }
```

### See Also

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


