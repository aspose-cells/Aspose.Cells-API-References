---
title: "ImageActiveXControl.IsAutoSize"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageActiveXControl-Eigenschaft. Gibt an, ob das Steuerelement automatisch die Größe ändert, um seinen gesamten Inhalt anzuzeigen"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/isautosize/
---
## ImageActiveXControl.IsAutoSize property

Gibt an, ob das Steuerelement automatisch die Größe ändert, um seinen gesamten Inhalt anzuzeigen.

```csharp
public override bool IsAutoSize { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyIsAutoSizeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein ImageActiveXControl zum Arbeitsblatt hinzu
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.Image, 
                5,  // left
                5,  // top
                100, // width
                100, // height
                0,   // imageWidth (0 for default)
                0    // imageHeight (0 for default)
            );
            Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl imageControl = 
                (Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl)shape.ActiveXControl;

            // Setze die Bilddaten (stelle sicher, dass die Bilddatei existiert)
            imageControl.Picture = File.ReadAllBytes("ControlPictureSizeMode.png");

            // Demonstriere die IsAutoSize-Eigenschaft
            imageControl.IsAutoSize = true; // Control will automatically resize to fit the image
            imageControl.PictureSizeMode = Aspose.Cells.Drawing.ActiveXControls.ControlPictureSizeMode.Zoom;

            // Speichere die Arbeitsmappe
            workbook.Save("ImageActiveXControlIsAutoSizeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


