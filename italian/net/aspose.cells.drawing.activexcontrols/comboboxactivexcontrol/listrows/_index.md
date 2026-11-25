---
title: "ComboBoxActiveXControl.ListRows"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ComboBoxActiveXControl. Rappresenta il numero massimo di righe da visualizzare nell'elenco"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/listrows/
---
## ComboBoxActiveXControl.ListRows property

Rappresenta il numero massimo di righe da visualizzare nell'elenco.

```csharp
public int ListRows { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyListRowsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ComboBox ActiveX con parametri di larghezza/altezza appropriati
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 10, 10, 150, 30, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Aggiungi elementi di esempio alla casella combinata usando ListFillRange
            comboBox.ListFillRange = "A1:A7";
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            worksheet.Cells["A5"].PutValue("Item 5");
            worksheet.Cells["A6"].PutValue("Item 6");
            worksheet.Cells["A7"].PutValue("Item 7");

            // Imposta la proprietà ListRows per controllare gli elementi visibili nel menu a discesa
            comboBox.ListRows = 4; // Only show 4 items at a time

            // Salva la cartella di lavoro
            workbook.Save("ComboBoxListRowsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


