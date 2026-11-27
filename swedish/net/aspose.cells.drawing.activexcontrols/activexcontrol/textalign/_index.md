---
title: "ActiveXControl.TextAlign"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ActiveXControl egenskap. Representerar hur texten som används av kontrollen ska justeras"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/activexcontrol/textalign/
---
## ActiveXControl.TextAlign property

Representerar hur texten som används av kontrollen ska justeras.

```csharp
public TextAlignmentType TextAlign { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlPropertyTextAlignDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till två kryssrute-ActiveX-kontroller
            Shape shape1 = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 0, 1, 0, 100, 30);
            Shape shape2 = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 0, 2, 0, 100, 30);

            // Hämta ActiveX-kontrollerna
            CheckBoxActiveXControl checkbox1 = (CheckBoxActiveXControl)shape1.ActiveXControl;
            CheckBoxActiveXControl checkbox2 = (CheckBoxActiveXControl)shape2.ActiveXControl;

            // Ställ in olika textjusteringar
            checkbox1.TextAlign = TextAlignmentType.Center;
            checkbox2.TextAlign = TextAlignmentType.Right;

            // Visa textjusteringsvärdena
            Console.WriteLine("Checkbox1 TextAlign: " + checkbox1.TextAlign);
            Console.WriteLine("Checkbox2 TextAlign: " + checkbox2.TextAlign);
        }
    }
}
```

### Se även

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


