---
title: "ToggleButtonActiveXControl.IsTripleState"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ToggleButtonActiveXControl Eigenschaft. Gibt an, wie das angegebene Steuerelement Null-Werte anzeigen wird"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/istriplestate/
---
## ToggleButtonActiveXControl.IsTripleState property

Gibt an, wie das angegebene Steuerelement Nullwerte anzeigen wird.

```csharp
public bool IsTripleState { get; set; }
```

### Hinweise

| **Einstellung** | **Beschreibung** |
| --- | --- |
| Wahr | Das Steuerelement durchläuft die Zustände für Ja-, Nein- und Nullwerte. Das Steuerelement erscheint abgedunkelt (grau), wenn seine Value‑Eigenschaft auf Null gesetzt ist. |
| Falsch | (Standard) Das Steuerelement durchläuft die Zustände für Ja- und Neinwerte. Nullwerte werden angezeigt, als wären sie Nein-Werte. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertyIsTripleStateDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein ToggleButton‑ActiveX‑Steuerelement hinzu
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ToggleButton, 1, 0, 1, 0, 100, 30);
            var toggleButton = (Aspose.Cells.Drawing.ActiveXControls.ToggleButtonActiveXControl)shape.ActiveXControl;

            // Setze die IsTripleState‑Eigenschaft auf true
            toggleButton.IsTripleState = true;
            Console.WriteLine("ToggleButton IsTripleState: " + toggleButton.IsTripleState);

            // Ändere die IsTripleState‑Eigenschaft auf false
            toggleButton.IsTripleState = false;
            Console.WriteLine("ToggleButton IsTripleState: " + toggleButton.IsTripleState);

            // Speichere die Arbeitsmappe
            workbook.Save("ToggleButtonIsTripleStateDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


