---
title: "RadioButton.IsChecked"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RadioButton. Indica se il pulsante di opzione è selezionato o meno"
type: docs
url: /it/net/aspose.cells.drawing/radiobutton/ischecked/
---
## RadioButton.IsChecked property

Indica se il radiobutton è selezionato o meno.

```csharp
public bool IsChecked { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class RadioButtonPropertyIsCheckedDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un pulsante di opzione al foglio di lavoro
            Shape shape = worksheet.Shapes.AddRadioButton(1, 0, 1, 0, 100, 100);
            RadioButton radioButton = (RadioButton)shape;
            
            // Imposta il testo del pulsante di opzione
            radioButton.Text = "Option 1";
            
            // Inizialmente non selezionato
            radioButton.IsChecked = false;
            Console.WriteLine("Radio button initially unchecked: " + radioButton.IsChecked);
            
            // Seleziona il pulsante di opzione
            radioButton.IsChecked = true;
            Console.WriteLine("Radio button after checking: " + radioButton.IsChecked);
            
            // Salva la cartella di lavoro
            workbook.Save("RadioButtonExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [RadioButton](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


