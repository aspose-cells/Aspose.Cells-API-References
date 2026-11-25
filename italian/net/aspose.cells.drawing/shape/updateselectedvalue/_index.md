---
title: "Shape.UpdateSelectedValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Shape. Aggiorna il valore selezionato con il valore della cella collegata"
type: docs
url: /it/net/aspose.cells.drawing/shape/updateselectedvalue/
---
## Shape.UpdateSelectedValue method

Aggiorna il valore selezionato con il valore della cella collegata.

```csharp
public void UpdateSelectedValue()
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodUpdateSelectedValueDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola alcuni dati di esempio
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = i + 1;
            }

            // Crea una forma ListBox
            Shape listBoxShape = worksheet.Shapes.AddListBox(2, 0, 2, 0, 130, 130);
            
            // Imposta l'intervallo di input e la cella collegata
            listBoxShape.SetInputRange("$A$1:$A$6", false, false);
            listBoxShape.SetLinkedCell("$A$12", false, true);

            // Ottieni l'oggetto ListBox
            ListBox listBox = (ListBox)listBoxShape;

            // Imposta il valore iniziale nella cella collegata e aggiorna la selezione
            worksheet.Cells["A12"].Value = 3;
            listBoxShape.UpdateSelectedValue();

            // Verifica la selezione
            if (listBox.IsSelected(2))
            {
                Console.WriteLine("Option 3 is selected");
            }

            // Cambia il valore e aggiorna nuovamente la selezione
            worksheet.Cells["A12"].Value = 4;
            listBoxShape.UpdateSelectedValue();

            if (listBox.IsSelected(3))
            {
                Console.WriteLine("Option 4 is selected");
            }
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


