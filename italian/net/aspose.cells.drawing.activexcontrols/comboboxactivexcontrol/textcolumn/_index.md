---
title: "ComboBoxActiveXControl.TextColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ComboBoxActiveXControl. Rappresenta la colonna in un ComboBox o ListBox da visualizzare all'utente"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/textcolumn/
---
## ComboBoxActiveXControl.TextColumn property

Rappresenta la colonna in un ComboBox o ListBox da visualizzare all'utente.

```csharp
public int TextColumn { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyTextColumnDemo
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

            // Configura le proprietà del combo box
            comboBox.ColumnCount = 2;
            comboBox.ListRows = 5;
            
            // Aggiungi elementi usando ListFillRange (alternativa a AddItem)
            worksheet.Cells["A1"].PutValue("Item1");
            worksheet.Cells["B1"].PutValue("Description1");
            worksheet.Cells["A2"].PutValue("Item2");
            worksheet.Cells["B2"].PutValue("Description2");
            worksheet.Cells["A3"].PutValue("Item3");
            worksheet.Cells["B3"].PutValue("Description3");
            comboBox.ListFillRange = "A1:B3";

            // Dimostra la proprietà TextColumn
            comboBox.TextColumn = 2; // Display second column (descriptions) as text
            comboBox.BoundColumn = 1; // But bind to first column (items)

            // Salva la cartella di lavoro
            workbook.Save("ComboBoxTextColumnDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


