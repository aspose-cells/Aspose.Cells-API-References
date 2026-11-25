---
title: "CalculationCell.Cell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CalculationCell. Restituisce l'oggetto Cell che viene calcolato"
type: docs
url: /it/net/aspose.cells/calculationcell/cell/
---
## CalculationCell.Cell property

Restituisce l'oggetto Cell che è in fase di calcolo.

```csharp
public Cell Cell { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CalculationCellPropertyCellDemo
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

                // Visualizza il valore della proprietà Cell
                Console.WriteLine("Cell Name: " + calcCell.Cell.Name);
                Console.WriteLine("Cell Value: " + calcCell.Cell.Value);
                Console.WriteLine("Cell StringValue: " + calcCell.Cell.StringValue);
                Console.WriteLine("Cell Row: " + calcCell.Cell.Row);
                Console.WriteLine("Cell Column: " + calcCell.Cell.Column);
                Console.WriteLine("Cell IsFormula: " + calcCell.Cell.IsFormula);

                // Dimostra le proprietà correlate per contesto
                Console.WriteLine("CellRow: " + calcCell.CellRow);
                Console.WriteLine("CellColumn: " + calcCell.CellColumn);

                // Salva la cartella di lavoro
                workbook.Save("CellDemo.xlsx");
                Console.WriteLine("Cell property demonstration completed successfully.");
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

* class [Cell](../../cell/)
* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


