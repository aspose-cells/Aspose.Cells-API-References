---
title: "ImageActiveXControl.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageActiveXControl. Ottiene il tipo del controllo ActiveX"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/type/
---
## ImageActiveXControl.Type property

Ottiene il tipo del controllo ActiveX.

```csharp
public override ControlType Type { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un controllo Image ActiveX
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 1, 1, 1, 1, 200, 100);
            ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;
            
            // Dimostra l'uso della proprietà Type
            Console.WriteLine("Control Type: " + imageControl.Type);
            
            // Imposta alcune proprietà
            imageControl.IsAutoSize = false;
            imageControl.BorderStyle = ControlBorderType.Single;
            imageControl.PictureSizeMode = ControlPictureSizeMode.Clip;
            
            // Salva la cartella di lavoro
            workbook.Save("ImageActiveXControlDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ControlType](../../controltype/)
* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


