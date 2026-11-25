---
title: "CalculationCell.CellRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CalculationCell. Ottiene l'indice di riga della cella"
type: docs
url: /it/net/aspose.cells/calculationcell/cellrow/
---
## CalculationCell.CellRow property

Restituisce l'indice della riga della cella.

```csharp
public int CellRow { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CalculationCellPropertyCellRowDemo
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

                // Visualizza il valore della proprietà CellRow
                Console.WriteLine("CellRow value: " + calcCell.CellRow);

                // Dimostra le proprietà correlate per contesto
                Console.WriteLine("CellColumn value: " + calcCell.CellColumn);
                Console.WriteLine("Cell Value: " + calcCell.Cell.Value);

                // Salva la cartella di lavoro
                workbook.Save("CellRowDemo.xlsx");
                Console.WriteLine("CellRow property demonstration completed successfully.");
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

* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


