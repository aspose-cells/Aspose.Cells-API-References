---
title: "ToggleButtonActiveXControl.Value"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ToggleButtonActiveXControl. Indica se il controllo è selezionato o meno"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/value/
---
## ToggleButtonActiveXControl.Value property

Indica se il controllo è selezionato o meno.

```csharp
public CheckValueType Value { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertyValueDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX ToggleButton
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 1, 1, 100, 30);
            ToggleButtonActiveXControl toggleButton = (ToggleButtonActiveXControl)shape.ActiveXControl;

            // Imposta il valore iniziale su Non selezionato
            toggleButton.Value = CheckValueType.UnChecked;

            // Verifica e cambia il valore se è Non selezionato
            if (toggleButton.Value == CheckValueType.UnChecked)
            {
                toggleButton.Value = CheckValueType.Checked;
            }

            // Salva la cartella di lavoro
            workbook.Save("ToggleButtonDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [CheckValueType](../../../aspose.cells.drawing/checkvaluetype/)
* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


