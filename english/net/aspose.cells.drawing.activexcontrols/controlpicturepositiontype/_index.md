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
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlsClassControlPicturePositionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 0, 1, 0, 100, 50);
            ToggleButtonActiveXControl activeXControl = (ToggleButtonActiveXControl)shape.ActiveXControl;

            activeXControl.Caption = "Demo Button";
            activeXControl.PicturePosition = ControlPicturePositionType.AboveLeft;
            activeXControl.IsAutoSize = true;

            workbook.Save("ActiveXControlDemo.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


