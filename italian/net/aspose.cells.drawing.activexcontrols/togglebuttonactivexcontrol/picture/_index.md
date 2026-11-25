---
title: "ToggleButtonActiveXControl.Picture"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ToggleButtonActiveXControl. Ottiene e imposta i dati dell'immagine"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/picture/
---
## ToggleButtonActiveXControl.Picture property

Ottiene e imposta i dati dell'immagine.

```csharp
public byte[] Picture { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertyPictureDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ToggleButton ActiveX e ottieni la sua proprietà ActiveXControl
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ToggleButton, 1, 1, 100, 30, 100, 30);
            var toggleButton = (Aspose.Cells.Drawing.ActiveXControls.ToggleButtonActiveXControl)shape.ActiveXControl;

            // Imposta l'immagine per il pulsante toggle
            byte[] data = File.ReadAllBytes("image.png");
            toggleButton.Picture = data;

            // Salva la cartella di lavoro
            workbook.Save("ToggleButtonWithPicture.xlsx");
        }
    }
}
```

### Vedi anche

* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


