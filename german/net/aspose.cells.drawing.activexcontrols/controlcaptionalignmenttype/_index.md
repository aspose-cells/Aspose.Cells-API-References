---
title: "Enum ControlCaptionAlignmentType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlCaptionAlignmentType enum. Gibt die Position der Beschriftung relativ zum Steuerelement an"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/controlcaptionalignmenttype/
---
## ControlCaptionAlignmentType enumeration

Stellt die Position der Beschriftung relativ zum Steuerelement dar.

```csharp
public enum ControlCaptionAlignmentType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Left | `0` | Die linke Seite des Steuerelements. |
| Right | `1` | Die rechte Seite des Steuerelements. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlCaptionAlignmentTypeDemo
    {
        public static void ControlCaptionAlignmentTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein CheckBox‑ActiveX‑Steuerelement zum Arbeitsblatt hinzu
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 5, 0, 1, 1, 100, 20);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Legen Sie Eigenschaften für die CheckBox fest
            checkBox.Caption = "Check Me!";
            checkBox.Alignment = ControlCaptionAlignmentType.Right;
            checkBox.IsWordWrapped = true;
            checkBox.Value = CheckValueType.Checked;

            // Fügen Sie ein RadioButton‑ActiveX‑Steuerelement zum Arbeitsblatt hinzu
            var shape2 = worksheet.Shapes.AddActiveXControl(ControlType.RadioButton, 10, 0, 1, 1, 100, 20);
            RadioButtonActiveXControl radioButton = (RadioButtonActiveXControl)shape2.ActiveXControl;

            // Legen Sie Eigenschaften für den RadioButton fest
            radioButton.Caption = "Select Me!";
            radioButton.Alignment = ControlCaptionAlignmentType.Left;
            radioButton.IsWordWrapped = true;

            // Speichere die Arbeitsmappe
            workbook.Save("ControlCaptionAlignmentTypeExample.xlsx");
            workbook.Save("ControlCaptionAlignmentTypeExample.pdf");
            // Ergebnisse ausgeben
            Console.WriteLine("CheckBox Alignment: " + checkBox.Alignment);
            Console.WriteLine("RadioButton Alignment: " + radioButton.Alignment);
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


