---
title: "ListBox.SelectionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListBox. Ottiene o imposta la modalità di selezione della list box specificata"
type: docs
url: /it/net/aspose.cells.drawing/listbox/selectiontype/
---
## ListBox.SelectionType property

Ottiene o imposta la modalità di selezione della casella di riepilogo specificata.

```csharp
public SelectionType SelectionType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxPropertySelectionTypeDemo
    {
        public static void Run()
        {
            // Crea una nuova Workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la list box
            sheet.Cells["A1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Finance");
            sheet.Cells["A3"].PutValue("MIS");
            sheet.Cells["A4"].PutValue("R&D");

            // Aggiungi una list box
            ListBox listBox = sheet.Shapes.AddListBox(1, 0, 2, 0, 100, 80);
            
            // Imposta le proprietà della list box
            listBox.InputRange = "A1:A4";
            listBox.LinkedCell = "B1";
            
            // Dimostra la proprietà SelectionType
            listBox.SelectionType = SelectionType.Single; // Only single selection allowed
            listBox.SelectedIndex = 1; // Select "Finance"

            // Salva la cartella di lavoro
            workbook.Save("ListBoxSelectionTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [SelectionType](../../selectiontype/)
* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


