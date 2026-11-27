---
title: "ToggleButtonActiveXControl.IsTripleState"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ToggleButtonActiveXControl-egenskap. Anger hur den angivna kontrollen visar Null‑värden"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/istriplestate/
---
## ToggleButtonActiveXControl.IsTripleState property

Anger hur den angivna kontrollen kommer att visa nullvärden.

```csharp
public bool IsTripleState { get; set; }
```

### Anmärkningar

| **Inställning** | **Beskrivning** |
| --- | --- |
| True | Kontrollen kommer att cykla genom tillstånd för Ja, Nej och Null‑värden. Kontrollen visas nedtonad (grå) när dess Value‑egenskap är satt till Null. |
| False | (Standard) Kontrollen kommer att cykla genom tillstånd för Ja‑ och Nej‑värden. Null‑värden visas som om de vore Nej‑värden. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertyIsTripleStateDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ToggleButton ActiveX-kontroll
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ToggleButton, 1, 0, 1, 0, 100, 30);
            var toggleButton = (Aspose.Cells.Drawing.ActiveXControls.ToggleButtonActiveXControl)shape.ActiveXControl;

            // Ange IsTripleState‑egenskap till true
            toggleButton.IsTripleState = true;
            Console.WriteLine("ToggleButton IsTripleState: " + toggleButton.IsTripleState);

            // Ändra IsTripleState‑egenskap till false
            toggleButton.IsTripleState = false;
            Console.WriteLine("ToggleButton IsTripleState: " + toggleButton.IsTripleState);

            // Spara arbetsboken
            workbook.Save("ToggleButtonIsTripleStateDemo.xlsx");
        }
    }
}
```

### Se även

* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


