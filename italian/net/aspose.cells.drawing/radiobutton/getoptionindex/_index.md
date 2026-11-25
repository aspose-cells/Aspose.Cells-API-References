---
title: "RadioButton.GetOptionIndex"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo RadioButton. Ottiene l'indice dell'opzione (basato su 1) in tutti i pulsanti di opzione del GroupBox che contiene questo pulsante di opzione"
type: docs
url: /it/net/aspose.cells.drawing/radiobutton/getoptionindex/
---
## RadioButton.GetOptionIndex method

Ottiene l'indice dell'opzione (basato su 1) in tutti i pulsanti di opzione del GroupBox che contiene questo pulsante di opzione.

```csharp
public int GetOptionIndex()
```

### Osservazioni

Se questo pulsante di opzione non è nel GroupBox, restituisce l'indice dell'opzione in tutti i pulsanti di opzione che non sono in alcun GroupBox

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class RadioButtonMethodGetOptionIndexDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un GroupBox per contenere i RadioButton
            GroupBox groupBox = worksheet.Shapes.AddGroupBox(1, 0, 100, 200, 100, 200);

            // Aggiungi tre pulsanti di opzione al group box
            RadioButton radioButton1 = (RadioButton)worksheet.Shapes.AddRadioButton(3, 0, 20, 100, 20, 100);
            RadioButton radioButton2 = (RadioButton)worksheet.Shapes.AddRadioButton(3, 0, 50, 100, 20, 100);
            RadioButton radioButton3 = (RadioButton)worksheet.Shapes.AddRadioButton(3, 0, 80, 100, 20, 100);

            // Imposta i pulsanti di opzione per far parte del group box
            radioButton1.Placement = PlacementType.FreeFloating;
            radioButton2.Placement = PlacementType.FreeFloating;
            radioButton3.Placement = PlacementType.FreeFloating;

            try
            {
                // Ottieni l'indice dell'opzione per ogni pulsante di opzione
                int index1 = radioButton1.GetOptionIndex();
                int index2 = radioButton2.GetOptionIndex();
                int index3 = radioButton3.GetOptionIndex();

                Console.WriteLine($"RadioButton1 Option Index: {index1}");
                Console.WriteLine($"RadioButton2 Option Index: {index2}");
                Console.WriteLine($"RadioButton3 Option Index: {index3}");

                // Seleziona il primo pulsante di opzione per dimostrare la selezione
                radioButton1.IsChecked = true;
                Console.WriteLine("RadioButton1 is checked");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetOptionIndex method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("RadioButtonMethodGetOptionIndexDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [RadioButton](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


