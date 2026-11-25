---
title: "Cell.GetDependentsInCalculation"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cell. Ottiene tutte le celle il cui risultato calcolato dipende da questa cella"
type: docs
url: /it/net/aspose.cells/cell/getdependentsincalculation/
---
## Cell.GetDependentsInCalculation method

Ottiene tutte le celle il cui risultato calcolato dipende da questa cella.

```csharp
public IEnumerator GetDependentsInCalculation(bool recursive)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ricorsivo | Booleano | Restituisce i dipendenti che non fanno riferimento a questa cella direttamente ma fanno riferimento ad altre foglie di questa cella |

### Valore di ritorno

Enumeratore per enumerare tutti i dipendenti (oggetti Cell)

### Osservazioni

Per utilizzare questo metodo, assicurati che la cartella di lavoro sia impostata con valore true per [`EnableCalculationChain`](../../formulasettings/enablecalculationchain/) e sia stata completamente calcolata con questa impostazione. Se non vi è alcun riferimento di formula a questa cella, verrà restituito null.

### Esempi

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetDependentsInCalculationWithBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            cells["A1"].Formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2";
            cells["A2"].Formula = "=IF(TRUE,B2,B1)";
            
            workbook.Settings.FormulaSettings.EnableCalculationChain = true;
            workbook.CalculateFormula();
            
            IEnumerator en = cells["B1"].GetDependentsInCalculation(false);
            Console.WriteLine("B1's calculation dependents:");
            while(en.MoveNext())
            {
                Cell c = (Cell)en.Current;
                Console.WriteLine(c.Name);
            }
            
            en = cells["B2"].GetDependentsInCalculation(false);
            Console.WriteLine("B2's calculation dependents:");
            while(en.MoveNext())
            {
                Cell c = (Cell)en.Current;
                Console.WriteLine(c.Name);
            }
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


