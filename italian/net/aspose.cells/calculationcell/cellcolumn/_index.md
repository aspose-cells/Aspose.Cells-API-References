---
title: "CalculationCell.CellColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CalculationCell. Restituisce l'indice della colonna della cella"
type: docs
url: /it/net/aspose.cells/calculationcell/cellcolumn/
---
## CalculationCell.CellColumn property

Restituisce l'indice della colonna della cella.

```csharp
public int CellColumn { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationCellPropertyCellColumnDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Inserisci alcuni dati e una formula semplice
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["B1"].Formula = "=A1*2";

            try
            {
                // Ottieni un'istanza di CalculationCell tramite reflection (il suo costruttore non è pubblico)
                CalculationCell calcCell = (CalculationCell)Activator.CreateInstance(
                    typeof(CalculationCell), 
                    nonPublic: true);

                // Leggi e visualizza il valore della proprietà CellColumn
                Console.WriteLine("CellColumn value: " + calcCell.CellColumn);

                // Dimostrazione aggiuntiva delle proprietà correlate (opzionale)
                Console.WriteLine("CellRow value: " + calcCell.CellRow);
                Console.WriteLine("Workbook is null: " + (calcCell.Workbook == null));
                Console.WriteLine("Worksheet is null: " + (calcCell.Worksheet == null));

                // Salva la cartella di lavoro (il file conterrà i dati aggiunti)
                workbook.Save("CellColumnDemo.xlsx");
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


