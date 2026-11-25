---
title: "ShapeCollection.UpdateSelectedValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeCollection. Aggiorna il valore selezionato con il valore della cella collegata o dell'intervallo della forma"
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/updateselectedvalue/
---
## ShapeCollection.UpdateSelectedValue method

Aggiorna il valore selezionato con il valore della cella collegata o dell'intervallo della forma.

```csharp
public void UpdateSelectedValue()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodUpdateSelectedValueDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi una forma (elenco a discesa) al foglio di lavoro
            Aspose.Cells.Drawing.ListBox listBox = (Aspose.Cells.Drawing.ListBox)worksheet.Shapes.AddListBox(0, 0, 100, 100, 3, 20);
            
            // Imposta gli elementi dell'elenco e il valore selezionato
            listBox.SetInputRange("A1:A3", false, false);
            listBox.SelectedIndex = 1;
            
            // Aggiorna il valore selezionato nella forma
            worksheet.Shapes.UpdateSelectedValue();
            
            // Salva la cartella di lavoro
            workbook.Save("ShapeCollectionUpdateSelectedValueDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


