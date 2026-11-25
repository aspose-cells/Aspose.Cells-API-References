---
title: "Cell.GetArrayRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cell. Ottiene l'intervallo dell'array se la formula della cella è una formula di matrice"
type: docs
url: /it/net/aspose.cells/cell/getarrayrange/
---
## Cell.GetArrayRange method

Ottiene l'intervallo di array se la formula della cella è una formula di matrice.

```csharp
public CellArea GetArrayRange()
```

### Valore di ritorno

L'intervallo dell'array.

### Osservazioni

Si applica solo quando la formula della cella è una formula di matrice

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetArrayRangeDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Imposta una formula di array dinamico nella cella A1
            Cell cell = cells[0, 0];
            string formula = "=SEQUENCE(3,2)";
            cell.SetDynamicArrayFormula(formula, new FormulaParseOptions(), false);
            
            // Calcola le formule
            wb.CalculateFormula();
            
            // Ottieni l'intervallo dell'array della formula dinamica
            CellArea arrayRange = cell.GetArrayRange();
            
            // Stampa le informazioni sull'intervallo dell'array
            Console.WriteLine("Array range for dynamic formula:");
            Console.WriteLine($"Start row: {arrayRange.StartRow}");
            Console.WriteLine($"Start column: {arrayRange.StartColumn}");
            Console.WriteLine($"End row: {arrayRange.EndRow}");
            Console.WriteLine($"End column: {arrayRange.EndColumn}");
            
            // Stampa i valori nell'intervallo dell'array
            Console.WriteLine("\nValues in the array range:");
            for (int r = arrayRange.StartRow; r <= arrayRange.EndRow; r++)
            {
                for (int c = arrayRange.StartColumn; c <= arrayRange.EndColumn; c++)
                {
                    Console.Write(cells[r, c].Value + "\t");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


