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
// Called: label.PicturePosition = ControlPicturePositionType.Center;
public static void Type_ControlPicturePositionType()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a Label ActiveX control to the worksheet
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 5, 0, 1, 1, 100, 20);
            LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;

            // Set properties for the Label
            label.Caption = &quot;Hello, Aspose!&quot;;
            label.PicturePosition = ControlPicturePositionType.Center;
            label.BorderOleColor = 0x000000; // Black color
            label.BorderStyle = ControlBorderType.Single;
            label.SpecialEffect = ControlSpecialEffectType.Flat;
            label.Accelerator = &apos;H&apos;;
            label.IsWordWrapped = true;
            label.IsEnabled = true;
            label.IsLocked = false;
            label.IsTransparent = false;
            label.IsAutoSize = true;
            label.IMEMode = InputMethodEditorMode.NoControl;
            label.TextAlign = TextAlignmentType.Center;
            label.ForeOleColor = 0x000000; // Black color
            label.BackOleColor = 0xFFFFFF; // White color
            label.IsVisible = true;
            label.Shadow = false;

            // Save the workbook
            workbook.Save(&quot;LabelActiveXControlDemo.xlsx&quot;);

            // Output the results
            Console.WriteLine(&quot;Label Caption: &quot; + label.Caption);
            Console.WriteLine(&quot;Label Picture Position: &quot; + label.PicturePosition);
            Console.WriteLine(&quot;Label Border Color: &quot; + label.BorderOleColor);
            Console.WriteLine(&quot;Label Border Style: &quot; + label.BorderStyle);
            Console.WriteLine(&quot;Label Special Effect: &quot; + label.SpecialEffect);
            Console.WriteLine(&quot;Label Accelerator: &quot; + label.Accelerator);
            Console.WriteLine(&quot;Label Is Word Wrapped: &quot; + label.IsWordWrapped);
            Console.WriteLine(&quot;Label Is Enabled: &quot; + label.IsEnabled);
            Console.WriteLine(&quot;Label Is Locked: &quot; + label.IsLocked);
            Console.WriteLine(&quot;Label Is Transparent: &quot; + label.IsTransparent);
            Console.WriteLine(&quot;Label Is Auto Size: &quot; + label.IsAutoSize);
            Console.WriteLine(&quot;Label IME Mode: &quot; + label.IMEMode);
            Console.WriteLine(&quot;Label Text Align: &quot; + label.TextAlign);
            Console.WriteLine(&quot;Label Fore Color: &quot; + label.ForeOleColor);
            Console.WriteLine(&quot;Label Back Color: &quot; + label.BackOleColor);
            Console.WriteLine(&quot;Label Is Visible: &quot; + label.IsVisible);
            Console.WriteLine(&quot;Label Shadow: &quot; + label.Shadow);
        }
```

### See Also

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


