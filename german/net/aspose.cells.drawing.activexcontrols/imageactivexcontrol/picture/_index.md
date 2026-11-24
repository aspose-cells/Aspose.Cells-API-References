---
title: "ImageActiveXControl.Picture"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageActiveXControl-Eigenschaft. Gibt die Bilddaten zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/picture/
---
## ImageActiveXControl.Picture property

Liest und setzt die Bilddaten.

```csharp
public byte[] Picture { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyPictureDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein Image‑ActiveX‑Steuerelement hinzu
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 1, 1, 100, 100, 100, 100);
            ImageActiveXControl imgControl = (ImageActiveXControl)shape.ActiveXControl;

            // Eigenschaften festlegen
            imgControl.PictureSizeMode = ControlPictureSizeMode.Stretch;
            imgControl.PictureAlignment = ControlPictureAlignmentType.TopLeft;
            imgControl.IsTiled = false;

            // Setze die Picture-Eigenschaft (unter Verwendung eines Beispielbild-Byte-Arrays)
            byte[] imageData = new byte[] { 0x00, 0x01, 0x02 }; // Sample image data
            imgControl.Picture = imageData;

            // Verifiziere, dass die Picture-Eigenschaft gesetzt wurde
            Console.WriteLine("Picture data length: " + imgControl.Picture.Length);

            // Speichere die Arbeitsmappe
            workbook.Save("ImageActiveXControlDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


