---
title: "LabelActiveXControl.Picture"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "LabelActiveXControl proprietà. Ottiene e imposta i dati dell'immagine"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/picture/
---
## LabelActiveXControl.Picture property

Ottiene e imposta i dati dell'immagine.

```csharp
public byte[] Picture { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.IO;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class LabelActiveXControlPropertyPictureDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX Label
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 1, 1, 1, 1, 100, 50);
            LabelActiveXControl labelControl = (LabelActiveXControl)shape.ActiveXControl;

            // Imposta le proprietà di base
            labelControl.Caption = "Sample Label";
            labelControl.PicturePosition = ControlPicturePositionType.LeftTop;

            // Carica un'immagine per la proprietà Picture
            string imagePath = "sample.jpg"; // Replace with actual image path
            if (File.Exists(imagePath))
            {
                labelControl.Picture = File.ReadAllBytes(imagePath);
                Console.WriteLine("Picture set successfully");
            }
            else
            {
                Console.WriteLine("Image file not found, using null picture");
                labelControl.Picture = null;
            }

            // Salva la cartella di lavoro
            workbook.Save("LabelActiveXControlDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


