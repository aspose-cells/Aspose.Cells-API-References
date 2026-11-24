---
title: "Enum ControlPicturePositionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlPicturePositionType enum. Stellt den Ort des Steuerelementbildes relativ zu seiner Beschriftung dar."
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/controlpicturepositiontype/
---
## ControlPicturePositionType enumeration

Stellt den Ort des Bildes des Steuerelements relativ zu seiner Beschriftung dar.

```csharp
public enum ControlPicturePositionType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| LeftTop | `131072` | Das Bild erscheint links von der Beschriftung. Die Beschriftung ist am oberen Rand des Bildes ausgerichtet. |
| LeftCenter | `327683` | Das Bild erscheint links von der Beschriftung. Die Beschriftung ist relativ zum Bild zentriert. |
| LeftBottom | `524294` | Das Bild erscheint links von der Beschriftung. Die Beschriftung ist am unteren Rand des Bildes ausgerichtet. |
| RightTop | `2` | Das Bild erscheint rechts von der Beschriftung. Die Beschriftung ist am oberen Rand des Bildes ausgerichtet. |
| RightCenter | `196613` | Das Bild erscheint rechts von der Beschriftung. Die Beschriftung ist relativ zum Bild zentriert. |
| RightBottom | `393224` | Das Bild erscheint rechts von der Beschriftung. Die Beschriftung ist am unteren Rand des Bildes ausgerichtet. |
| AboveLeft | `393216` | Das Bild erscheint über der Beschriftung. Die Beschriftung ist am linken Rand des Bildes ausgerichtet. |
| AboveCenter | `458753` | Das Bild erscheint über der Beschriftung. Die Beschriftung ist unterhalb des Bildes zentriert. |
| AboveRight | `524290` | Das Bild erscheint über der Beschriftung. Die Beschriftung ist am rechten Rand des Bildes ausgerichtet. |
| BelowLeft | `6` | Das Bild erscheint unter der Beschriftung. Die Beschriftung ist am linken Rand des Bildes ausgerichtet. |
| BelowCenter | `65543` | Das Bild erscheint unter der Beschriftung. Die Beschriftung ist über dem Bild zentriert. |
| BelowRight | `131080` | Das Bild erscheint unter der Beschriftung. Die Beschriftung ist am rechten Rand des Bildes ausgerichtet. |
| Center | `262148` | Das Bild erscheint in der Mitte des Steuerelements. Die Beschriftung ist horizontal und vertikal zentriert über dem Bild. |

### Beispiele

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

### Siehe auch

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


