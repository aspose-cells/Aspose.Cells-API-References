---
title: "Enum ControlCaptionAlignmentType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlCaptionAlignmentType enum. Rappresenta la posizione della didascalia rispetto al controllo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/controlcaptionalignmenttype/
---
## ControlCaptionAlignmentType enumeration

Rappresenta la posizione della Caption rispetto al controllo.

```csharp
public enum ControlCaptionAlignmentType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Left | `0` | Il lato sinistro del controllo. |
| Right | `1` | Il lato destro del controllo. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX CheckBox al foglio di lavoro
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 5, 0, 1, 1, 100, 20);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Imposta le proprietà per il CheckBox
            checkBox.Caption = "Check Me!";
            checkBox.Alignment = ControlCaptionAlignmentType.Right;
            checkBox.IsWordWrapped = true;
            checkBox.Value = CheckValueType.Checked;

            // Aggiungi un controllo ActiveX RadioButton al foglio di lavoro
            var shape2 = worksheet.Shapes.AddActiveXControl(ControlType.RadioButton, 10, 0, 1, 1, 100, 20);
            RadioButtonActiveXControl radioButton = (RadioButtonActiveXControl)shape2.ActiveXControl;

            // Imposta le proprietà per il RadioButton
            radioButton.Caption = "Select Me!";
            radioButton.Alignment = ControlCaptionAlignmentType.Left;
            radioButton.IsWordWrapped = true;

            // Salva la cartella di lavoro
            workbook.Save("ControlCaptionAlignmentTypeExample.xlsx");
            workbook.Save("ControlCaptionAlignmentTypeExample.pdf");
            // Restituisci i risultati
            Console.WriteLine("CheckBox Alignment: " + checkBox.Alignment);
            Console.WriteLine("RadioButton Alignment: " + radioButton.Alignment);
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


