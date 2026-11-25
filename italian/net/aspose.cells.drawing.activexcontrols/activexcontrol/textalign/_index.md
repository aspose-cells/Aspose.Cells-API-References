---
title: "ActiveXControl.TextAlign"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ActiveXControl. Rappresenta come allineare il testo utilizzato dal controllo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/activexcontrol/textalign/
---
## ActiveXControl.TextAlign property

Rappresenta come allineare il testo utilizzato dal controllo.

```csharp
public TextAlignmentType TextAlign { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi due controlli ActiveX checkbox
            Shape shape1 = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 0, 1, 0, 100, 30);
            Shape shape2 = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 0, 2, 0, 100, 30);

            // Ottieni i controlli ActiveX
            CheckBoxActiveXControl checkbox1 = (CheckBoxActiveXControl)shape1.ActiveXControl;
            CheckBoxActiveXControl checkbox2 = (CheckBoxActiveXControl)shape2.ActiveXControl;

            // Imposta diversi allineamenti del testo
            checkbox1.TextAlign = TextAlignmentType.Center;
            checkbox2.TextAlign = TextAlignmentType.Right;

            // Visualizza i valori di allineamento del testo
            Console.WriteLine("Checkbox1 TextAlign: " + checkbox1.TextAlign);
            Console.WriteLine("Checkbox2 TextAlign: " + checkbox2.TextAlign);
        }
    }
}
```

### Vedi anche

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


