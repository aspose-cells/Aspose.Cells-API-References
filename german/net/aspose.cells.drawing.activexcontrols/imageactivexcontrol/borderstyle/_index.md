---
title: "ImageActiveXControl.BorderStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageActiveXControl-Eigenschaft. Gibt den Typ des vom Steuerelement verwendeten Rahmens zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/borderstyle/
---
## ImageActiveXControl.BorderStyle property

Liest und schreibt den Typ des vom Steuerelement verwendeten Rahmens.

```csharp
public ControlBorderType BorderStyle { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyBorderStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.Image, 
                5, 5, 100, 100, 200, 200);
            Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl imageControl = 
                (Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl)shape.ActiveXControl;

            // Setze den Rahmenstil und demonstriere seine Verwendung
            imageControl.BorderStyle = Aspose.Cells.Drawing.ActiveXControls.ControlBorderType.Single;
            imageControl.BorderOleColor = 0x000000; // Black border

            // Setze ein Beispielbild (stelle sicher, dass diese Datei in deinem Ausführungsverzeichnis existiert)
            if (File.Exists("sample.png"))
            {
                imageControl.Picture = File.ReadAllBytes("sample.png");
            }

            workbook.Save("ImageActiveXControlBorderStyleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ControlBorderType](../../controlbordertype/)
* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


