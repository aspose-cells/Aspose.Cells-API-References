---
title: "ActiveXControl.IMEMode"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ActiveXControl-egenskap. Hämtar och anger standardkörtidsläget för inmatningsmetodredigeraren för kontrollen när den får fokus"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/activexcontrol/imemode/
---
## ActiveXControl.IMEMode property

Hämtar och anger standardkörningsläget för inmatningsmetodredigeraren för kontrollen när den får fokus.

```csharp
public InputMethodEditorMode IMEMode { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ToggleButton ActiveX-kontroll med korrekta koordinater
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.ToggleButton, 
                1, 1,  // Upper-left row/column
                1, 1,  // Upper-left row/column offsets
                100, 50);  // Width and height
            ToggleButtonActiveXControl toggleButton = (ToggleButtonActiveXControl)shape.ActiveXControl;

            // Ställ in egenskaper inklusive IMEMode
            toggleButton.Caption = "ToggleButton1";
            toggleButton.PicturePosition = ControlPicturePositionType.AboveCenter;
            toggleButton.SpecialEffect = ControlSpecialEffectType.Sunken;
            toggleButton.IMEMode = InputMethodEditorMode.NoControl;

            // Verifiera och skriv ut IMEMode-egenskapen
            Console.WriteLine("ToggleButton IMEMode: " + toggleButton.IMEMode);

            // Spara arbetsboken
            workbook.Save("ActiveXControlIMEModeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [InputMethodEditorMode](../../inputmethodeditormode/)
* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


