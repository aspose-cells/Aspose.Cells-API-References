---
title: "Enum ControlSpecialEffectType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlSpecialEffectType enum. Rappresenta il tipo di effetto speciale"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/controlspecialeffecttype/
---
## ControlSpecialEffectType enumeration

Rappresenta il tipo di effetto speciale.

```csharp
public enum ControlSpecialEffectType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Flat | `0` | Piatto |
| Raised | `1` | In rilievo |
| Sunken | `2` | Incassato |
| Etched | `3` | Inciso |
| Bump | `6` | In rilievo |

### Esempi

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
            // Inizializza una nuova cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX CheckBox
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 0, 1, 0, 100, 50);
            CheckBoxActiveXControl checkBoxControl = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Imposta le proprietà del controllo ActiveX CheckBox
            checkBoxControl.Caption = "Example CheckBox";
            checkBoxControl.SpecialEffect = ControlSpecialEffectType.Raised;

            // Aggiungi un controllo ActiveX ComboBox
            shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 3, 0, 3, 0, 100, 50);
            ComboBoxActiveXControl comboBoxControl = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Imposta le proprietà del controllo ActiveX ComboBox
            comboBoxControl.SpecialEffect = ControlSpecialEffectType.Sunken;
            comboBoxControl.ListWidth = 100;
            comboBoxControl.ListRows = 5;

            // Aggiungi un controllo ActiveX TextBox
            shape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 5, 0, 5, 0, 100, 50);
            TextBoxActiveXControl textBoxControl = (TextBoxActiveXControl)shape.ActiveXControl;

            // Imposta le proprietà del controllo ActiveX TextBox
            textBoxControl.Text = "Example TextBox";
            textBoxControl.SpecialEffect = ControlSpecialEffectType.Bump;

            // Salva la cartella di lavoro
            workbook.Save("ControlSpecialEffectTypeExample.xlsx");
            workbook.Save("ControlSpecialEffectTypeExample.pdf");
            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


