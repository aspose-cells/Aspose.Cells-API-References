---
title: Enum ControlPicturePositionType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.ActiveXControls.ControlPicturePositionType enum. Represents the location of the controls picture relative to its caption
type: docs
url: /net/aspose.cells.drawing.activexcontrols/controlpicturepositiontype/
---
## ControlPicturePositionType enumeration

Represents the location of the control's picture relative to its caption.

```csharp
public enum ControlPicturePositionType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| LeftTop | `131072` | The picture appears to the left of the caption. The caption is aligned with the top of the picture. |
| LeftCenter | `327683` | The picture appears to the left of the caption. The caption is centered relative to the picture. |
| LeftBottom | `524294` | The picture appears to the left of the caption. The caption is aligned with the bottom of the picture. |
| RightTop | `2` | The picture appears to the right of the caption. The caption is aligned with the top of the picture. |
| RightCenter | `196613` | The picture appears to the right of the caption. The caption is centered relative to the picture. |
| RightBottom | `393224` | The picture appears to the right of the caption. The caption is aligned with the bottom of the picture. |
| AboveLeft | `393216` | The picture appears above the caption. The caption is aligned with the left edge of the picture. |
| AboveCenter | `458753` | The picture appears above the caption. The caption is centered below the picture. |
| AboveRight | `524290` | The picture appears above the caption. The caption is aligned with the right edge of the picture. |
| BelowLeft | `6` | The picture appears below the caption. The caption is aligned with the left edge of the picture. |
| BelowCenter | `65543` | The picture appears below the caption. The caption is centered above the picture. |
| BelowRight | `131080` | The picture appears below the caption. The caption is aligned with the right edge of the picture. |
| Center | `262148` | The picture appears in the center of the control. The caption is centered horizontally and vertically on top of the picture. |

### Examples

```csharp
// Called: activeXControl.PicturePosition = ControlPicturePositionType.AboveLeft;
public static void ActiveXControls_Type_ControlPicturePositionType()
        {
            // Initialize a new workbook.
            Workbook workbook = new Workbook();

            // Add a ToggleButtonActiveXControl.
            Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 0, 1, 0, 100, 50);
            ToggleButtonActiveXControl activeXControl = (ToggleButtonActiveXControl)shape.ActiveXControl;

            // Setting properties
            activeXControl.Caption = "ExampleButton";
            activeXControl.PicturePosition = ControlPicturePositionType.AboveLeft;
            activeXControl.SpecialEffect = ControlSpecialEffectType.Bump;
            activeXControl.Accelerator = '\0';
            activeXControl.Value = CheckValueType.Checked;
            activeXControl.IsTripleState = false;
            activeXControl.IsEnabled = true;
            activeXControl.IsLocked = false;
            activeXControl.IsTransparent = true;
            activeXControl.IsAutoSize = true;
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

            // Save the Excel file.
            workbook.Save("ToggleButtonActiveXControlExample.xlsx");
        }
```

### See Also

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


