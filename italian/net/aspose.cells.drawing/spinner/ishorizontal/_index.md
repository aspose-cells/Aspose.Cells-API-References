---
title: "Spinner.IsHorizontal"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Spinner. Indica se si tratta di una barra di scorrimento orizzontale"
type: docs
url: /it/net/aspose.cells.drawing/spinner/ishorizontal/
---
## Spinner.IsHorizontal property

Indica se questa è una barra di scorrimento orizzontale.

```csharp
public bool IsHorizontal { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class SpinnerPropertyIsHorizontalDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Aggiungi una forma spinner al foglio di lavoro
                Spinner spinner = worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 30);
                
                // Imposta le proprietà del spinner
                spinner.Min = 0;
                spinner.Max = 100;
                spinner.IncrementalChange = 5;
                spinner.CurrentValue = 50;
                
                // Dimostra la proprietà IsHorizontal (lettura e scrittura)
                Console.WriteLine("Initial IsHorizontal value: " + spinner.IsHorizontal);
                
                // Attiva/disattiva l'orientamento
                spinner.IsHorizontal = !spinner.IsHorizontal;
                Console.WriteLine("Modified IsHorizontal value: " + spinner.IsHorizontal);
                
                // Salva la cartella di lavoro
                workbook.Save("SpinnerIsHorizontalDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


