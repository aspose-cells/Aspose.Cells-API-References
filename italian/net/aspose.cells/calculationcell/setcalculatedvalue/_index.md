---
title: "CalculationCell.SetCalculatedValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CalculationCell. Imposta il valore calcolato per la cella"
type: docs
url: /it/net/aspose.cells/calculationcell/setcalculatedvalue/
---
## CalculationCell.SetCalculatedValue method

Imposta il valore calcolato per la cella.

```csharp
public void SetCalculatedValue(object v)
```

### Osservazioni

L'utente può impostare il risultato calcolato con questo metodo per ignorare il calcolo automatico della cella.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CalculationCellMethodSetCalculatedValueWithObjectDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["B1"].Formula = "=A1*2";

            try
            {
                // Crea un'istanza di CalculationCell usando la riflessione poiché il costruttore non è pubblico.
                CalculationCell calcCell = (CalculationCell)Activator.CreateInstance(
                    typeof(CalculationCell),
                    BindingFlags.NonPublic | BindingFlags.Instance,
                    null,
                    new object[] { workbook, worksheet, 0, 1, worksheet.Cells["B1"] },
                    null);

                // Imposta un valore calcolato usando il metodo SetCalculatedValue
                calcCell.SetCalculatedValue(42); // Using an integer value as the Object parameter

                // Visualizza le informazioni sulla cella
                Console.WriteLine("Cell Row: " + calcCell.CellRow);
                Console.WriteLine("Cell Column: " + calcCell.CellColumn);
                Console.WriteLine("SetCalculatedValue method called successfully with value: 42");

                // Salva la cartella di lavoro
                workbook.Save("SetCalculatedValueDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetCalculatedValue: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


