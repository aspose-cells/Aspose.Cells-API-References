---
title: "Enum ControlPictureSizeMode"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlPictureSizeMode enum. Gibt an, wie das Bild angezeigt wird."
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/controlpicturesizemode/
---
## ControlPictureSizeMode enumeration

Stellt dar, wie das Bild angezeigt wird.

```csharp
public enum ControlPictureSizeMode
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Clip | `0` | Schneidet jeden Teil des Bildes ab, der größer als die Grenzen des Steuerelements ist. |
| Stretch | `1` | Streckt das Bild, um den Bereich des Steuerelements auszufüllen. Diese Einstellung verzerrt das Bild in horizontaler oder vertikaler Richtung. |
| Zoom | `3` | Vergrößert das Bild, verzerrt es jedoch weder in horizontaler noch in vertikaler Richtung. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System.IO;

    public class ControlPictureSizeModeDemo
    {
        public static void ControlPictureSizeModeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Bild zum Arbeitsblatt hinzu
            int pictureIndex = worksheet.Pictures.Add(1, 1, "ControlPictureSizeMode.png");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Füge ein ImageActiveXControl zum Arbeitsblatt hinzu
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 5, 5, 5,5,100, 100);
            ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;

            // Setze die Bilddaten für das ImageActiveXControl
            imageControl.Picture = File.ReadAllBytes("ControlPictureSizeMode.png");

            // Setze den PictureSizeMode auf Zoom
            imageControl.PictureSizeMode = ControlPictureSizeMode.Zoom;

            // Setze weitere Eigenschaften des ImageActiveXControl
            imageControl.IsAutoSize = true;
            imageControl.BorderStyle = ControlBorderType.Single;
            imageControl.BorderOleColor = 0x000000; // Black color
            imageControl.SpecialEffect = ControlSpecialEffectType.Flat;
            imageControl.PictureAlignment = ControlPictureAlignmentType.Center;
            imageControl.IsTiled = false;

            // Speichere die Arbeitsmappe
            workbook.Save("ControlPictureSizeModeExample.xlsx");
            workbook.Save("ControlPictureSizeModeExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


