---
title: "CheckBoxActiveXControl.IsTripleState"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CheckBoxActiveXControl egenskap. Anger hur den angivna kontrollen kommer att visa Null‑värden"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/istriplestate/
---
## CheckBoxActiveXControl.IsTripleState property

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
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertyIsTripleStateDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en CheckBox ActiveX‑kontroll med alla nödvändiga parametrar
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 1, 100, 30, 100, 30);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Konfigurera grundläggande egenskaper
            checkBox.Caption = "Triple State Demo";
            
            // Demonstrera IsTripleState‑egenskap
            checkBox.IsTripleState = true; // Enable three states: Checked, Unchecked, and Indeterminate
            checkBox.Value = CheckValueType.Mixed; // Set to indeterminate state

            // Spara arbetsboken
            workbook.Save("CheckBoxTripleStateDemo.xlsx");
        }
    }
}
```

### Se även

* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


