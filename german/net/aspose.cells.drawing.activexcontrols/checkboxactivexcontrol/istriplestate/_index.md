---
title: "CheckBoxActiveXControl.IsTripleState"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CheckBoxActiveXControl-Eigenschaft. Gibt an, wie das angegebene Steuerelement Nullwerte anzeigt"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/istriplestate/
---
## CheckBoxActiveXControl.IsTripleState property

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
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertyIsTripleStateDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein CheckBox ActiveX-Steuerelement mit allen erforderlichen Parametern hinzu
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 1, 100, 30, 100, 30);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Grundlegende Eigenschaften konfigurieren
            checkBox.Caption = "Triple State Demo";
            
            // Demonstrieren Sie die IsTripleState-Eigenschaft
            checkBox.IsTripleState = true; // Enable three states: Checked, Unchecked, and Indeterminate
            checkBox.Value = CheckValueType.Mixed; // Set to indeterminate state

            // Speichere die Arbeitsmappe
            workbook.Save("CheckBoxTripleStateDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


