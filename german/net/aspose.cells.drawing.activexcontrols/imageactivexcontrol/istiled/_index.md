---
title: "ImageActiveXControl.IsTiled"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageActiveXControl-Eigenschaft. Gibt an, ob das Bild über den Hintergrund gekachelt wird"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/istiled/
---
## ImageActiveXControl.IsTiled property

Gibt an, ob das Bild über den Hintergrund gekachelt wird.

```csharp
public bool IsTiled { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyIsTiledDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Image ActiveX-Steuerelement zum Arbeitsblatt hinzu
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 5, 0, 1, 1, 100, 100);
            ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;

            // IsTiled-Eigenschaft und weitere Eigenschaften festlegen
            imageControl.IsTiled = true;
            imageControl.PictureSizeMode = ControlPictureSizeMode.Stretch;

            // Laden Sie ein Bild aus einer Datei (ersetzen Sie den Pfad durch Ihren eigenen Bildpfad)
            byte[] imageData = File.ReadAllBytes("demo.jpg");
            imageControl.Picture = imageData;

            // Speichere die Arbeitsmappe
            workbook.Save("ImageActiveXControlIsTiledDemo.xlsx");

            Console.WriteLine($"IsTiled property set to: {imageControl.IsTiled}");
        }
    }
}
```

### Siehe auch

* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


