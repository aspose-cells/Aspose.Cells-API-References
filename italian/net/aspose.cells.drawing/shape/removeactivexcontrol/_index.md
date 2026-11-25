---
title: "Shape.RemoveActiveXControl"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Shape. Rimuove il controllo ActiveX"
type: docs
url: /it/net/aspose.cells.drawing/shape/removeactivexcontrol/
---
## Shape.RemoveActiveXControl method

Rimuovi il controllo ActiveX.

```csharp
public void RemoveActiveXControl()
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodRemoveActiveXControlDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma che conterrà il controllo ActiveX
            Shape shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.CommandButton, 
                1, 1, 1, 1, 100, 50);
            
            // Rimuovi il controllo ActiveX se esiste
            if (shape.ActiveXControl != null)
            {
                shape.RemoveActiveXControl();
                Console.WriteLine("ActiveX control removed successfully.");
            }
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


