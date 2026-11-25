---
title: "ActiveXControlBase.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ActiveXControlBase. Ottiene il tipo del controllo ActiveX"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/type/
---
## ActiveXControlBase.Type property

Ottiene il tipo del controllo ActiveX.

```csharp
public abstract ControlType Type { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX Label con i parametri corretti
            Shape labelShape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 1, 1, 1, 100, 50, 0);
            LabelActiveXControl labelControl = (LabelActiveXControl)labelShape.ActiveXControl;
            labelControl.Caption = "Label_ActiveX";

            // Dimostra l'uso della proprietà Type
            if (labelShape.ActiveXControl.Type == ControlType.Label)
            {
                Console.WriteLine("The control is a Label type");
                labelControl.Caption = labelControl.Caption.Replace("Label_", "MyChangedLabel_");
            }

            // Salva e verifica
            workbook.Save("output.xlsx");
            Console.WriteLine("Label caption changed to: " + labelControl.Caption);
        }
    }
}
```

### Vedi anche

* enum [ControlType](../../controltype/)
* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


