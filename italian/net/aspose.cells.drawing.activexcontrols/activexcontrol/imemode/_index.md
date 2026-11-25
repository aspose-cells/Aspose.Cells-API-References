---
title: "ActiveXControl.IMEMode"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ActiveXControl. Ottiene e imposta la modalità di runtime predefinita dell'Input Method Editor per il controllo quando riceve il focus"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/activexcontrol/imemode/
---
## ActiveXControl.IMEMode property

Ottiene e imposta la modalità di esecuzione predefinita dell'Input Method Editor per il controllo quando riceve il focus.

```csharp
public InputMethodEditorMode IMEMode { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlPropertyIMEModeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX ToggleButton con le coordinate corrette
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.ToggleButton, 
                1, 1,  // Upper-left row/column
                1, 1,  // Upper-left row/column offsets
                100, 50);  // Width and height
            ToggleButtonActiveXControl toggleButton = (ToggleButtonActiveXControl)shape.ActiveXControl;

            // Imposta le proprietà includendo IMEMode
            toggleButton.Caption = "ToggleButton1";
            toggleButton.PicturePosition = ControlPicturePositionType.AboveCenter;
            toggleButton.SpecialEffect = ControlSpecialEffectType.Sunken;
            toggleButton.IMEMode = InputMethodEditorMode.NoControl;

            // Verifica e restituisci la proprietà IMEMode
            Console.WriteLine("ToggleButton IMEMode: " + toggleButton.IMEMode);

            // Salva la cartella di lavoro
            workbook.Save("ActiveXControlIMEModeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [InputMethodEditorMode](../../inputmethodeditormode/)
* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


