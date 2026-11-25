---
title: "CheckBoxActiveXControl.Caption"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CheckBoxActiveXControl. Ottiene e imposta il testo descrittivo che appare su un controllo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/caption/
---
## CheckBoxActiveXControl.Caption property

Ottiene e imposta il testo descrittivo che appare su un controllo.

```csharp
public string Caption { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertyCaptionDemo
    {
        public static void Run()
        {
            // Inizializza una nuova cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX CheckBox
            Shape shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.CheckBox, 1, 0, 1, 0, 100, 50);
            CheckBoxActiveXControl checkBoxControl = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Imposta e dimostra la proprietà Caption
            checkBoxControl.Caption = "Sample CheckBox Caption";
            checkBoxControl.Value = CheckValueType.Checked;  // Fixed: Using correct enum value

            // Salva la cartella di lavoro
            workbook.Save("CheckBoxCaptionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


