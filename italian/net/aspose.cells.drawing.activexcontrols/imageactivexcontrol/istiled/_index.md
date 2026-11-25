---
title: "ImageActiveXControl.IsTiled"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageActiveXControl. Indica se l'immagine è ripetuta sullo sfondo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/istiled/
---
## ImageActiveXControl.IsTiled property

Indica se l'immagine è ripetuta sullo sfondo.

```csharp
public bool IsTiled { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo Image ActiveX al foglio di lavoro
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 5, 0, 1, 1, 100, 100);
            ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;

            // Imposta la proprietà IsTiled e altre proprietà
            imageControl.IsTiled = true;
            imageControl.PictureSizeMode = ControlPictureSizeMode.Stretch;

            // Carica un'immagine da file (sostituisci con il percorso della tua immagine)
            byte[] imageData = File.ReadAllBytes("demo.jpg");
            imageControl.Picture = imageData;

            // Salva la cartella di lavoro
            workbook.Save("ImageActiveXControlIsTiledDemo.xlsx");

            Console.WriteLine($"IsTiled property set to: {imageControl.IsTiled}");
        }
    }
}
```

### Vedi anche

* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


