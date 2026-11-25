---
title: "ToggleButtonActiveXControl.Accelerator"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ToggleButtonActiveXControl. Ottiene e imposta il tasto di accelerazione per il controllo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/accelerator/
---
## ToggleButtonActiveXControl.Accelerator property

Ottiene e imposta il tasto di accelerazione per il controllo.

```csharp
public char Accelerator { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertyAcceleratorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX ToggleButton con i parametri corretti
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 100, 30, 100, 30);
            ToggleButtonActiveXControl toggleButton = (ToggleButtonActiveXControl)shape.ActiveXControl;

            // Imposta la proprietà Accelerator
            toggleButton.Accelerator = 'A';
            Console.WriteLine("ToggleButton Accelerator set to: " + toggleButton.Accelerator);

            // Cancella la proprietà Accelerator
            toggleButton.Accelerator = '\0';
            Console.WriteLine("ToggleButton Accelerator cleared: " + (toggleButton.Accelerator == '\0' ? "True" : "False"));
        }
    }
}
```

### Vedi anche

* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


