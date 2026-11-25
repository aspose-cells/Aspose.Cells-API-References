---
title: "ImageActiveXControl.Picture"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageActiveXControl. Ottiene e imposta i dati dell'immagine"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/picture/
---
## ImageActiveXControl.Picture property

Ottiene e imposta i dati dell'immagine.

```csharp
public byte[] Picture { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX Image
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 1, 1, 100, 100, 100, 100);
            ImageActiveXControl imgControl = (ImageActiveXControl)shape.ActiveXControl;

            // Imposta le proprietà
            imgControl.PictureSizeMode = ControlPictureSizeMode.Stretch;
            imgControl.PictureAlignment = ControlPictureAlignmentType.TopLeft;
            imgControl.IsTiled = false;

            // Imposta la proprietà Picture (usando un array di byte dell'immagine di esempio)
            byte[] imageData = new byte[] { 0x00, 0x01, 0x02 }; // Sample image data
            imgControl.Picture = imageData;

            // Verifica che la proprietà Picture sia stata impostata
            Console.WriteLine("Picture data length: " + imgControl.Picture.Length);

            // Salva la cartella di lavoro
            workbook.Save("ImageActiveXControlDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


