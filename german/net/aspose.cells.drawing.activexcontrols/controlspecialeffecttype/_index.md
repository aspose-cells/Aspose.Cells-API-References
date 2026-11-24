---
title: "Enum ControlSpecialEffectType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlSpecialEffectType enum. Stellt den Typ des Spezialeffekts dar"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/controlspecialeffecttype/
---
## ControlSpecialEffectType enumeration

Stellt den Typ des Spezialeffekts dar.

```csharp
public enum ControlSpecialEffectType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Flat | `0` | Flach |
| Raised | `1` | Erhoben |
| Sunken | `2` | Eingesunken |
| Etched | `3` | Geätzt |
| Bump | `6` | Erhebung |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlSpecialEffectTypeDemo
    {
        public static void ControlSpecialEffectTypeExample()
        {
            // Initialisieren Sie ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein CheckBox‑ActiveX‑Steuerelement hinzufügen
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 0, 1, 0, 100, 50);
            CheckBoxActiveXControl checkBoxControl = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Eigenschaften des CheckBox‑ActiveX‑Steuerelements festlegen
            checkBoxControl.Caption = "Example CheckBox";
            checkBoxControl.SpecialEffect = ControlSpecialEffectType.Raised;

            // Ein ComboBox‑ActiveX‑Steuerelement hinzufügen
            shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 3, 0, 3, 0, 100, 50);
            ComboBoxActiveXControl comboBoxControl = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Eigenschaften des ComboBox‑ActiveX‑Steuerelements festlegen
            comboBoxControl.SpecialEffect = ControlSpecialEffectType.Sunken;
            comboBoxControl.ListWidth = 100;
            comboBoxControl.ListRows = 5;

            // Ein TextBox‑ActiveX‑Steuerelement hinzufügen
            shape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 5, 0, 5, 0, 100, 50);
            TextBoxActiveXControl textBoxControl = (TextBoxActiveXControl)shape.ActiveXControl;

            // Eigenschaften des TextBox‑ActiveX‑Steuerelements festlegen
            textBoxControl.Text = "Example TextBox";
            textBoxControl.SpecialEffect = ControlSpecialEffectType.Bump;

            // Speichere die Arbeitsmappe
            workbook.Save("ControlSpecialEffectTypeExample.xlsx");
            workbook.Save("ControlSpecialEffectTypeExample.pdf");
            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


