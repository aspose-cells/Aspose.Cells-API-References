---
title: "ComboBoxActiveXControl.MaxLength"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ComboBoxActiveXControl property. Ottiene e imposta il numero massimo di caratteri"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/maxlength/
---
## ComboBoxActiveXControl.MaxLength property

Ottiene e imposta il numero massimo di caratteri

```csharp
public int MaxLength { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyMaxLengthDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX ComboBox al foglio di lavoro
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 
                5, 0, 100, 20, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Imposta la proprietà MaxLength e altre proprietà essenziali
            comboBox.MaxLength = 10; // Restrict input to 10 characters
            comboBox.ListRows = 5;
            comboBox.IsEditable = true;
            comboBox.Value = "Test";

            // Salva la cartella di lavoro
            workbook.Save("ComboBoxMaxLengthDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


