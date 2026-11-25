---
title: "CommandButtonActiveXControl.Picture"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "CommandButtonActiveXControl property. Ottiene e imposta i dati dell'immagine"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/picture/
---
## CommandButtonActiveXControl.Picture property

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
    public class CommandButtonActiveXControlPropertyPictureDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una forma per ospitare il controllo ActiveX con tutti i parametri richiesti
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.CommandButton, 
                1,  // top row
                1,  // left column
                0,  // top position
                0,  // left position
                100, // width
                30); // height
                
            CommandButtonActiveXControl button = (CommandButtonActiveXControl)shape.ActiveXControl;

            // Imposta le proprietà
            button.Caption = "Click Me";
            button.PicturePosition = ControlPicturePositionType.AboveCenter;

            // Imposta l'immagine (un array di byte vuoto rappresenta nessuna immagine)
            button.Picture = new byte[0];

            // Salva la cartella di lavoro
            workbook.Save("CommandButtonWithPicture.xlsx");

            // Verifica la proprietà picture
            Console.WriteLine("Picture is null: " + (button.Picture == null));
        }
    }
}
```

### Vedi anche

* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


