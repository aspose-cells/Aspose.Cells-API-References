---
title: "Classe CalculationCell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.CalculationCell. Rappresenta i dati rilevanti per il calcolo di una cella che è in fase di calcolo"
type: docs
url: /it/net/aspose.cells/calculationcell/
---
## CalculationCell class

Rappresenta i dati rilevanti al calcolo di una cella che è in fase di calcolo.

```csharp
public class CalculationCell
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Cell](../../aspose.cells/calculationcell/cell/) { get; } | Restituisce l'oggetto Cell che è in fase di calcolo. |
| [CellColumn](../../aspose.cells/calculationcell/cellcolumn/) { get; } | Restituisce l'indice della colonna della cella. |
| [CellRow](../../aspose.cells/calculationcell/cellrow/) { get; } | Restituisce l'indice della riga della cella. |
| [Workbook](../../aspose.cells/calculationcell/workbook/) { get; } | Restituisce l'oggetto Workbook. |
| [Worksheet](../../aspose.cells/calculationcell/worksheet/) { get; } | Restituisce l'oggetto Worksheet in cui si trova la cella. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SetCalculatedValue](../../aspose.cells/calculationcell/setcalculatedvalue/)(object) | Imposta il valore calcolato per la cella. |

### Osservazioni

L'utente non dovrebbe modificare alcun dato nel Workbook durante il processo di calcolo della formula, altrimenti potrebbero verificarsi risultati inattesi o un'Exception. Pertanto, tutti gli oggetti forniti da questa classe (come l'oggetto Cell di [`Cell`](./cell/)) sono destinati solo alla lettura.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CellsClassCalculationCellDemo
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

                // Visualizza le proprietà di base
                Console.WriteLine($"Cell Row: {calcCell.CellRow}");
                Console.WriteLine($"Cell Column: {calcCell.CellColumn}");
                Console.WriteLine($"Cell Value: {calcCell.Cell.Value}");
                Console.WriteLine($"Workbook Name: {calcCell.Workbook.FileName}");
                Console.WriteLine($"Worksheet Name: {calcCell.Worksheet.Name}");

                // Salva la cartella di lavoro
                workbook.Save("CalculationCellDemo.xlsx");
                Console.WriteLine("CalculationCell demonstration completed successfully.");
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

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


