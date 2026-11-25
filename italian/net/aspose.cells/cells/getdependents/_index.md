---
title: "Cells.GetDependents"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Ottieni tutte le celle che fanno riferimento alla cella specifica"
type: docs
url: /it/net/aspose.cells/cells/getdependents/
---
## Cells.GetDependents method

Ottieni tutte le celle che fanno riferimento alla cella specifica.

```csharp
public Cell[] GetDependents(bool isAll, int row, int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isAll | Booleano | Indica se controllare altri fogli di lavoro |
| riga | Int32 | L'indice della riga. |
| colonna | Int32 | L'indice della colonna. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetDependentsWithBooleanInt32Int32Demo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Configura formule di esempio e valori
            cells["A1"].PutValue(10);
            cells["B1"].Formula = "=A1*2";
            cells["C1"].Formula = "=A1+B1";
            cells["D1"].Formula = "=B1*3";
            cells["F4"].Formula = "=A1*5";

            // Calcola le formule
            workbook.CalculateFormula();

            // Ottieni i dipendenti diretti della cella A1 (riga 0, colonna 0)
            Cell[] directDependents = cells.GetDependents(false, 0, 0);
            Console.WriteLine("Direct dependents of A1:");
            foreach (Cell cell in directDependents)
            {
                Console.WriteLine(cell.Name);
            }

            // Ottieni tutti i dipendenti (inclusi indiretti) della cella A1 (riga 0, colonna 0)
            Cell[] allDependents = cells.GetDependents(true, 0, 0);
            Console.WriteLine("\nAll dependents of A1:");
            foreach (Cell cell in allDependents)
            {
                Console.WriteLine(cell.Name);
            }
        }
    }
}
```

### Vedi anche

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


