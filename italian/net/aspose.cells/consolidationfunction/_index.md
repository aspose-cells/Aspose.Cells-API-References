---
title: "Enum ConsolidationFunction"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.ConsolidationFunction. Rappresenta la funzione di consolidamento"
type: docs
url: /it/net/aspose.cells/consolidationfunction/
---
## ConsolidationFunction enumeration

Rappresenta la funzione di consolidamento.

```csharp
public enum ConsolidationFunction
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Sum | `0` | Rappresenta la funzione Sum. |
| Count | `1` | Rappresenta la funzione Count. |
| Average | `2` | Rappresenta la funzione Average. |
| Max | `3` | Rappresenta la funzione Max. |
| Min | `4` | Rappresenta la funzione Min. |
| Product | `5` | Rappresenta la funzione Product. |
| CountNums | `6` | Rappresenta la funzione Count Nums. |
| StdDev | `7` | Rappresenta la funzione StdDev. |
| StdDevp | `8` | Rappresenta la funzione StdDevp. |
| Var | `9` | Rappresenta la funzione Var. |
| Varp | `10` | Rappresenta la funzione Varp. |
| DistinctCount | `11` | Rappresenta la funzione Distinct Count. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConsolidationFunctionDemo
    {
        public static void ConsolidationFunctionExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Definisci l'area della cella per il subtotale
            CellArea cellArea = new CellArea
            {
                StartRow = 1,
                StartColumn = 0,
                EndRow = 3,
                EndColumn = 1
            };

            // Applica il subtotale con la funzione Sum
            worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Sum, new int[] { 1 });

            // Applica il subtotale con la funzione Average
            worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Average, new int[] { 1 });

            // Applica il subtotale con la funzione Max
            worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Max, new int[] { 1 });

            // Applica il subtotale con la funzione Min
            worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Min, new int[] { 1 });

            // Salva la cartella di lavoro
            workbook.Save("ConsolidationFunctionExample.xlsx");
            workbook.Save("ConsolidationFunctionExample.pdf");

            // Restituisci i risultati
            Console.WriteLine("Workbook saved with subtotals applied.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


