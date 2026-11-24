---
title: "Shape.RemoveActiveXControl"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Methode. Entfernt das ActiveX-Steuerelement"
type: docs
url: /de/net/aspose.cells.drawing/shape/removeactivexcontrol/
---
## Shape.RemoveActiveXControl method

Entfernt das ActiveX-Steuerelement.

```csharp
public void RemoveActiveXControl()
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein Shape hinzu, das das ActiveX-Steuerelement enthält
            Shape shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.CommandButton, 
                1, 1, 1, 1, 100, 50);
            
            // Entfernen Sie das ActiveX-Steuerelement, falls es existiert
            if (shape.ActiveXControl != null)
            {
                shape.RemoveActiveXControl();
                Console.WriteLine("ActiveX control removed successfully.");
            }
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


