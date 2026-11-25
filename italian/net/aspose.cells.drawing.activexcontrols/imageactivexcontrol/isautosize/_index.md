---
title: "ImageActiveXControl.IsAutoSize"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageActiveXControl. Indica se il controllo ridimensionerà automaticamente per visualizzare tutto il contenuto"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/isautosize/
---
## ImageActiveXControl.IsAutoSize property

Indica se il controllo ridimensionerà automaticamente per visualizzare tutto il contenuto.

```csharp
public override bool IsAutoSize { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un ImageActiveXControl al foglio di lavoro
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

            // Imposta i dati dell'immagine (assicurati che il file immagine esista)
            imageControl.Picture = File.ReadAllBytes("ControlPictureSizeMode.png");

            // Dimostra la proprietà IsAutoSize
            imageControl.IsAutoSize = true; // Control will automatically resize to fit the image
            imageControl.PictureSizeMode = Aspose.Cells.Drawing.ActiveXControls.ControlPictureSizeMode.Zoom;

            // Salva la cartella di lavoro
            workbook.Save("ImageActiveXControlIsAutoSizeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


