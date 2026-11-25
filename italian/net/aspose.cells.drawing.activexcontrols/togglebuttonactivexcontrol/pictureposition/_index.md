---
title: "ToggleButtonActiveXControl.PicturePosition"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ToggleButtonActiveXControl. Ottiene e imposta la posizione dell'immagine del controllo rispetto alla sua didascalia"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/pictureposition/
---
## ToggleButtonActiveXControl.PicturePosition property

Ottiene e imposta la posizione dell'immagine del controllo rispetto alla sua didascalia.

```csharp
public ControlPicturePositionType PicturePosition { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertyPicturePositionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ToggleButton ActiveX con tutti i parametri richiesti
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 1, 100, 30, 0);
            var control = shape.ActiveXControl;

            if (control is ToggleButtonActiveXControl toggleButton)
            {
                // Imposta la proprietà PicturePosition
                toggleButton.PicturePosition = ControlPicturePositionType.AboveLeft;

                // Imposta altre proprietà per dimostrare la funzionalità
                toggleButton.Caption = "Toggle Button";
                toggleButton.Picture = new byte[0]; // Empty picture for demo
            }

            // Salva la cartella di lavoro
            workbook.Save("ToggleButtonActiveXControlDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ControlPicturePositionType](../../controlpicturepositiontype/)
* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


