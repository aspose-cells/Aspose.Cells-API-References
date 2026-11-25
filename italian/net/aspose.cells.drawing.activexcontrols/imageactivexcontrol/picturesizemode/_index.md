---
title: "ImageActiveXControl.PictureSizeMode"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageActiveXControl. Ottiene e imposta come visualizzare l'immagine"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/picturesizemode/
---
## ImageActiveXControl.PictureSizeMode property

Ottiene e imposta come visualizzare l'immagine.

```csharp
public ControlPictureSizeMode PictureSizeMode { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo Image ActiveX al foglio di lavoro
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 1, 1, 200, 200, 0, 0);
            ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;

            // Imposta PictureSizeMode e altre proprietà
            imageControl.PictureSizeMode = ControlPictureSizeMode.Stretch;
            
            // Carica un'immagine di esempio (sostituisci con il percorso della tua immagine)
            string imagePath = "sample.jpg";
            if (File.Exists(imagePath))
            {
                byte[] imageData = File.ReadAllBytes(imagePath);
                imageControl.Picture = imageData;
            }

            // Salva la cartella di lavoro
            workbook.Save("ImageActiveXControlDemo.xlsx");

            // Restituisci il valore di PictureSizeMode
            Console.WriteLine($"PictureSizeMode: {imageControl.PictureSizeMode}");
        }
    }
}
```

### Vedi anche

* enum [ControlPictureSizeMode](../../controlpicturesizemode/)
* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


