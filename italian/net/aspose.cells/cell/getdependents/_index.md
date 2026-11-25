---
title: "Cell.GetDependents"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cell. Ottieni tutte le celle la cui formula fa riferimento direttamente a questa cella"
type: docs
url: /it/net/aspose.cells/cell/getdependents/
---
## Cell.GetDependents method

Ottieni tutte le celle la cui formula fa riferimento direttamente a questa cella.

```csharp
public Cell[] GetDependents(bool isAll)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isAll | Booleano | Indica se controllare le formule in altri fogli di lavoro |

### Osservazioni

Se un riferimento contenente questa cella appare nella formula di un'altra cella, quella cella verrà considerata dipendente di questa cella, indipendentemente dal fatto che il riferimento o questa cella siano utilizzati o meno durante il calcolo. Per esempio, sebbene la cella A2 nella formula "=IF(TRUE,A1,A2)" non sia utilizzata durante il calcolo, questa formula viene comunque considerata dipendente di A2. Per ottenere le formule i cui risultati calcolati dipendono da questa cella, si prega di utilizzare [`GetDependentsInCalculation`](../getdependentsincalculation/). Quando si tracciano i dipendenti per una cella, tutte le formule nella cartella di lavoro o nel foglio di lavoro verranno analizzate e verificate. Pertanto è un processo che richiede tempo. Se l'utente deve tracciare i dipendenti per molte celle, l'uso di questo metodo causerà scarse prestazioni. Per motivi di prestazioni, l'utente dovrebbe utilizzare [`GetDependentsInCalculation`](../getdependentsincalculation/) invece. Oppure, l'utente può prima raccogliere la mappa dei precedenti di tutte le celle con [`GetPrecedents`](../getprecedents/), e poi costruire la mappa dei dipendenti in base alla mappa dei precedenti.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetDependentsWithBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta le formule che fanno riferimento a B1
            cells["A1"].Formula = "=B1+5";
            cells["A2"].Formula = "=B1*2";
            cells["A3"].Formula = "=SUM(B1:B3)";

            // Calcola le formule
            workbook.CalculateFormula();

            // Ottieni tutte le celle che dipendono da B1 (ricorsivo)
            Cell[] dependents = cells["B1"].GetDependents(true);

            Console.WriteLine("Cells dependent on B1:");
            foreach (Cell cell in dependents)
            {
                Console.WriteLine(cell.Name + ": " + cell.Formula);
            }
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


