---
title: "ScrollBarActiveXControl.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ScrollBarActiveXControl. Ottiene il tipo del controllo ActiveX"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/type/
---
## ScrollBarActiveXControl.Type property

Ottiene il tipo del controllo ActiveX.

```csharp
public override ControlType Type { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ScrollBarActiveXControlPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX ScrollBar con i parametri corretti
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ScrollBar, 1, 1, 1, 100, 20, 0);
            ScrollBarActiveXControl scrollBar = (ScrollBarActiveXControl)shape.ActiveXControl;

            // Verifica il tipo di controllo usando la proprietà Type
            if (scrollBar.Type == ControlType.ScrollBar)
            {
                // Imposta proprietà specifiche di ScrollBar
                scrollBar.Max = 100;
                scrollBar.Min = 0;
                scrollBar.Position = 50;
            }

            // Salva la cartella di lavoro
            workbook.Save("ScrollBarActiveXControlDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ControlType](../../controltype/)
* class [ScrollBarActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


