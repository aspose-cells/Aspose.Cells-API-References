---
title: "ComboBoxActiveXControl.SelectionMargin"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ComboBoxActiveXControl. Indica se l'utente può selezionare una riga di testo facendo clic nella zona a sinistra del testo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/selectionmargin/
---
## ComboBoxActiveXControl.SelectionMargin property

Indica se l'utente può selezionare una riga di testo facendo clic nella zona a sinistra del testo.

```csharp
public bool SelectionMargin { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertySelectionMarginDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Dimostra la proprietà SelectionMargin
            comboBox.SelectionMargin = false;
            Console.WriteLine("SelectionMargin set to: " + comboBox.SelectionMargin);

            // Attiva/disattiva e dimostra di nuovo
            comboBox.SelectionMargin = true;
            Console.WriteLine("SelectionMargin now set to: " + comboBox.SelectionMargin);

            workbook.Save("ComboBoxSelectionMarginDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


