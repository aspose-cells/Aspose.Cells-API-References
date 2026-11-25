---
title: "Enum ControlPictureSizeMode"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlPictureSizeMode enum. Rappresenta come visualizzare l'immagine"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/controlpicturesizemode/
---
## ControlPictureSizeMode enumeration

Rappresenta come visualizzare l'immagine.

```csharp
public enum ControlPictureSizeMode
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Clip | `0` | Ritaglia qualsiasi parte dell'immagine più grande dei confini del controllo. |
| Stretch | `1` | Allunga l'immagine per riempire l'area del controllo. Questa impostazione distorce l'immagine sia in direzione orizzontale che verticale. |
| Zoom | `3` | Ingrandisce l'immagine, ma non la distorce né in direzione orizzontale né verticale. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System.IO;

    public class ControlPictureSizeModeDemo
    {
        public static void ControlPictureSizeModeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un'immagine al foglio di lavoro
            int pictureIndex = worksheet.Pictures.Add(1, 1, "ControlPictureSizeMode.png");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Aggiungi un ImageActiveXControl al foglio di lavoro
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 5, 5, 5,5,100, 100);
            ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;

            // Imposta i dati dell'immagine per l'ImageActiveXControl
            imageControl.Picture = File.ReadAllBytes("ControlPictureSizeMode.png");

            // Imposta il PictureSizeMode su Zoom
            imageControl.PictureSizeMode = ControlPictureSizeMode.Zoom;

            // Imposta altre proprietà dell'ImageActiveXControl
            imageControl.IsAutoSize = true;
            imageControl.BorderStyle = ControlBorderType.Single;
            imageControl.BorderOleColor = 0x000000; // Black color
            imageControl.SpecialEffect = ControlSpecialEffectType.Flat;
            imageControl.PictureAlignment = ControlPictureAlignmentType.Center;
            imageControl.IsTiled = false;

            // Salva la cartella di lavoro
            workbook.Save("ControlPictureSizeModeExample.xlsx");
            workbook.Save("ControlPictureSizeModeExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


