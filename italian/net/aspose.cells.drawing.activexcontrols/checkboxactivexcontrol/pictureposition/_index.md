---
title: "CheckBoxActiveXControl.PicturePosition"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CheckBoxActiveXControl. Ottiene e imposta la posizione dell'immagine del controllo rispetto alla sua didascalia"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/pictureposition/
---
## CheckBoxActiveXControl.PicturePosition property

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
    public class CheckBoxActiveXControlPropertyPicturePositionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo CheckBox ActiveX con tutti i parametri richiesti
            var shape = worksheet.Shapes.AddActiveXControl(
                ControlType.CheckBox, 
                10,  // left
                10,  // top
                150, // width
                30,  // height
                0,   // leftOffset
                0    // topOffset
            );
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Configura le proprietà del CheckBox
            checkBox.Caption = "Sample CheckBox";
            checkBox.PicturePosition = ControlPicturePositionType.Center;
            checkBox.IsAutoSize = true;

            // Salva la cartella di lavoro
            workbook.Save("CheckBoxPicturePositionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ControlPicturePositionType](../../controlpicturepositiontype/)
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


