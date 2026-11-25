---
title: "ActiveXControl.IsTransparent"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ActiveXControl. Indica se il controllo è trasparente"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/activexcontrol/istransparent/
---
## ActiveXControl.IsTransparent property

Indica se il controllo è trasparente.

```csharp
public bool IsTransparent { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlPropertyIsTransparentDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una forma per ospitare il controllo ActiveX con tutti i parametri richiesti
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.Label, 
                1, 1, 200, 50, 
                0, 0); // Adding missing parameters for upperLeftRow, upperLeftColumn, height, width, left, top

            LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;

            // Imposta le proprietà del controllo
            label.Caption = "Sample Label";
            label.IsTransparent = false; // Demonstrating IsTransparent property

            // Verifica e restituisci la proprietà IsTransparent
            Console.WriteLine("Label IsTransparent property: " + label.IsTransparent);

            // Modifica la trasparenza e verifica nuovamente
            label.IsTransparent = true;
            Console.WriteLine("Label IsTransparent property after change: " + label.IsTransparent);

            // Salva la cartella di lavoro
            workbook.Save("ActiveXControlIsTransparentDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


