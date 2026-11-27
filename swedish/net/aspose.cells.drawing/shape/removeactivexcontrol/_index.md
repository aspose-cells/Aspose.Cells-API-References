---
title: "Shape.RemoveActiveXControl"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape‑metod. Ta bort activeX‑kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing/shape/removeactivexcontrol/
---
## Shape.RemoveActiveXControl method

Ta bort ActiveX-kontrollen.

```csharp
public void RemoveActiveXControl()
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en shape som kommer att innehålla ActiveX‑kontrollen
            Shape shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.CommandButton, 
                1, 1, 1, 1, 100, 50);
            
            // Ta bort ActiveX‑kontrollen om den finns
            if (shape.ActiveXControl != null)
            {
                shape.RemoveActiveXControl();
                Console.WriteLine("ActiveX control removed successfully.");
            }
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


