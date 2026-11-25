---
title: "ComboBoxActiveXControl.HideSelection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ComboBoxActiveXControl property. Indica se il testo selezionato nel controllo appare evidenziato quando il controllo non ha il focus"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/hideselection/
---
## ComboBoxActiveXControl.HideSelection property

Indica se il testo selezionato nel controllo appare evidenziato quando il controllo non ha il focus.

```csharp
public bool HideSelection { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyHideSelectionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ComboBox ActiveX con tutti i parametri richiesti
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 
                10, 10, 150, 30, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Configura le proprietà di base
            comboBox.ListRows = 5;
            comboBox.Value = "Select an item";
            
            // Aggiungi elementi di esempio usando il nome corretto della proprietà
            comboBox.ListFillRange = "A1:A3"; // Alternative way to set items
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");

            // Dimostra la proprietà HideSelection
            comboBox.HideSelection = true; // Text won't show selection highlight when control loses focus

            // Salva la cartella di lavoro
            workbook.Save("ComboBoxHideSelectionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


