---
title: "ImageActiveXControl.PictureSizeMode"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageActiveXControl-Eigenschaft. Gibt zurück, wie das Bild angezeigt wird, und legt dies fest"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/picturesizemode/
---
## ImageActiveXControl.PictureSizeMode property

Liest und setzt, wie das Bild angezeigt wird.

```csharp
public ControlPictureSizeMode PictureSizeMode { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyPictureSizeModeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Image ActiveX-Steuerelement zum Arbeitsblatt hinzu
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 1, 1, 200, 200, 0, 0);
            ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;

            // Setze PictureSizeMode und andere Eigenschaften
            imageControl.PictureSizeMode = ControlPictureSizeMode.Stretch;
            
            // Lade ein Beispielbild (ersetze es durch deinen eigenen Bildpfad)
            string imagePath = "sample.jpg";
            if (File.Exists(imagePath))
            {
                byte[] imageData = File.ReadAllBytes(imagePath);
                imageControl.Picture = imageData;
            }

            // Speichere die Arbeitsmappe
            workbook.Save("ImageActiveXControlDemo.xlsx");

            // Gib den Wert von PictureSizeMode aus
            Console.WriteLine($"PictureSizeMode: {imageControl.PictureSizeMode}");
        }
    }
}
```

### Siehe auch

* enum [ControlPictureSizeMode](../../controlpicturesizemode/)
* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


