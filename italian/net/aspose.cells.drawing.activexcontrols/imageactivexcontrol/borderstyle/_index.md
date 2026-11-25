---
title: "ImageActiveXControl.BorderStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageActiveXControl. Ottiene e imposta il tipo di bordo utilizzato dal controllo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/borderstyle/
---
## ImageActiveXControl.BorderStyle property

Ottiene e imposta il tipo di bordo utilizzato dal controllo.

```csharp
public ControlBorderType BorderStyle { get; set; }
```

### Esempi

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

            // Imposta lo stile del bordo e dimostra il suo utilizzo
            imageControl.BorderStyle = Aspose.Cells.Drawing.ActiveXControls.ControlBorderType.Single;
            imageControl.BorderOleColor = 0x000000; // Black border

            // Imposta l'immagine di esempio (assicurati che questo file esista nella directory di esecuzione)
            if (File.Exists("sample.png"))
            {
                imageControl.Picture = File.ReadAllBytes("sample.png");
            }

            workbook.Save("ImageActiveXControlBorderStyleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ControlBorderType](../../controlbordertype/)
* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


