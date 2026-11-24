---
title: "Enum ControlPictureAlignmentType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlPictureAlignmentType‑Enum. Stellt die Ausrichtung des Bildes innerhalb des Formulars oder Bildes dar."
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/controlpicturealignmenttype/
---
## ControlPictureAlignmentType enumeration

Stellt die Ausrichtung des Bildes innerhalb des Formulars oder Bildes dar.

```csharp
public enum ControlPictureAlignmentType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| TopLeft | `0` | Die obere linke Ecke. |
| TopRight | `1` | Die obere rechte Ecke. |
| Center | `2` | Die Mitte. |
| BottomLeft | `3` | Die untere linke Ecke. |
| BottomRight | `4` | Die untere rechte Ecke. |

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ActiveXControlsClassControlPictureAlignmentTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein ImageActiveXControl mit allen erforderlichen Parametern hinzu
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.Image, 
                10,  // left
                10,  // top
                200, // width
                200, // height
                0,   // imageWidth
                0    // imageHeight
            );
            Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl imageControl = 
                (Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl)shape.ActiveXControl;

            // Legen Sie Bildeigenschaften fest
            imageControl.Picture = File.ReadAllBytes("sample.png");
            imageControl.PictureAlignment = Aspose.Cells.Drawing.ActiveXControls.ControlPictureAlignmentType.Center;
            imageControl.PictureSizeMode = Aspose.Cells.Drawing.ActiveXControls.ControlPictureSizeMode.Stretch;

            // Speichere die Arbeitsmappe
            workbook.Save("ImageControlDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


