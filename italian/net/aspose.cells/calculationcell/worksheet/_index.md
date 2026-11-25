---
title: "CalculationCell.Worksheet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CalculationCell. Ottiene l'oggetto Worksheet in cui si trova la cella"
type: docs
url: /it/net/aspose.cells/calculationcell/worksheet/
---
## CalculationCell.Worksheet property

Restituisce l'oggetto Worksheet in cui si trova la cella.

```csharp
public Worksheet Worksheet { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CalculationCellPropertyWorksheetDemo
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

                // Visualizza il valore della proprietà Worksheet
                Console.WriteLine("Worksheet Name: " + calcCell.Worksheet.Name);
                Console.WriteLine("Worksheet Index: " + calcCell.Worksheet.Index);
                Console.WriteLine("Worksheet Type: " + calcCell.Worksheet.Type);

                // Dimostra altre proprietà correlate
                Console.WriteLine("Cell Row: " + calcCell.CellRow);
                Console.WriteLine("Cell Column: " + calcCell.CellColumn);

                // Salva la cartella di lavoro
                workbook.Save("WorksheetDemo.xlsx");
                Console.WriteLine("Worksheet property demonstration completed successfully.");
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

* class [Worksheet](../../worksheet/)
* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


