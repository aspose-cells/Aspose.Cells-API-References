---
title: "CheckBoxActiveXControl.IsTripleState"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CheckBoxActiveXControl. Indica come il controllo specificato visualizzerà i valori Null"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/istriplestate/
---
## CheckBoxActiveXControl.IsTripleState property

Indica come il controllo specificato visualizzerà i valori Null.

```csharp
public bool IsTripleState { get; set; }
```

### Osservazioni

| **Impostazione** | **Description** |
| --- | --- |
| True | Il controllo ciclerà attraverso gli stati per i valori Sì, No e Null. Il controllo appare attenuato (grigio) quando la sua proprietà Value è impostata su Null. |
| False | (Predefinito) Il controllo ciclerà attraverso gli stati per i valori Sì e No. I valori Null vengono visualizzati come se fossero valori No. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo CheckBox ActiveX con tutti i parametri richiesti
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 1, 100, 30, 100, 30);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Configura le proprietà di base
            checkBox.Caption = "Triple State Demo";
            
            // Dimostra la proprietà IsTripleState
            checkBox.IsTripleState = true; // Enable three states: Checked, Unchecked, and Indeterminate
            checkBox.Value = CheckValueType.Mixed; // Set to indeterminate state

            // Salva la cartella di lavoro
            workbook.Save("CheckBoxTripleStateDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


