---
title: "ActiveXControl.IMEMode"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ActiveXControl-Eigenschaft. Ruft den Standardlaufzeitmodus des Eingabemethoden-Editors für das Steuerelement ab und legt ihn fest, wenn es den Fokus erhält"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/activexcontrol/imemode/
---
## ActiveXControl.IMEMode property

Liest und setzt den Standard‑Laufzeitmodus des Eingabemethoden-Editors für das Steuerelement, wenn es den Fokus erhält.

```csharp
public InputMethodEditorMode IMEMode { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein ToggleButton-ActiveX-Steuerelement mit korrekten Koordinaten hinzufügen
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.ToggleButton, 
                1, 1,  // Upper-left row/column
                1, 1,  // Upper-left row/column offsets
                100, 50);  // Width and height
            ToggleButtonActiveXControl toggleButton = (ToggleButtonActiveXControl)shape.ActiveXControl;

            // Eigenschaften einschließlich IMEMode festlegen
            toggleButton.Caption = "ToggleButton1";
            toggleButton.PicturePosition = ControlPicturePositionType.AboveCenter;
            toggleButton.SpecialEffect = ControlSpecialEffectType.Sunken;
            toggleButton.IMEMode = InputMethodEditorMode.NoControl;

            // Die IMEMode-Eigenschaft überprüfen und ausgeben
            Console.WriteLine("ToggleButton IMEMode: " + toggleButton.IMEMode);

            // Speichere die Arbeitsmappe
            workbook.Save("ActiveXControlIMEModeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [InputMethodEditorMode](../../inputmethodeditormode/)
* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


