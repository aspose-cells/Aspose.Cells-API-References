---
title: "Enum ControlPictureAlignmentType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Drawing.ActiveXControls.ControlPictureAlignmentType. Rappresenta l'allineamento dell'immagine all'interno del Form o dell'Image"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/controlpicturealignmenttype/
---
## ControlPictureAlignmentType enumeration

Rappresenta l'allineamento dell'immagine all'interno del Form o Image.

```csharp
public enum ControlPictureAlignmentType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| TopLeft | `0` | L'angolo in alto a sinistra. |
| TopRight | `1` | L'angolo in alto a destra. |
| Center | `2` | Il centro. |
| BottomLeft | `3` | L'angolo in basso a sinistra. |
| BottomRight | `4` | L'angolo in basso a destra. |

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ActiveXControlsClassControlPictureAlignmentTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un ImageActiveXControl con tutti i parametri richiesti
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.Image, 
                10,  // left
                10,  // top
                200, // width
                200, // height
                0,   // imageWidth
                0    // imageHeight
            );
            Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl imageControl = 
                (Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl)shape.ActiveXControl;

            // Imposta le proprietà dell'immagine
            imageControl.Picture = File.ReadAllBytes("sample.png");
            imageControl.PictureAlignment = Aspose.Cells.Drawing.ActiveXControls.ControlPictureAlignmentType.Center;
            imageControl.PictureSizeMode = Aspose.Cells.Drawing.ActiveXControls.ControlPictureSizeMode.Stretch;

            // Salva la cartella di lavoro
            workbook.Save("ImageControlDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


