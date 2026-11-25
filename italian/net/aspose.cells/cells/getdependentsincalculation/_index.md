---
title: "Cells.GetDependentsInCalculation"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Ottiene tutte le celle il cui risultato calcolato dipende da una cella specifica"
type: docs
url: /it/net/aspose.cells/cells/getdependentsincalculation/
---
## Cells.GetDependentsInCalculation method

Restituisce tutte le celle il cui risultato calcolato dipende dalla cella specifica.

```csharp
public IEnumerator GetDependentsInCalculation(int row, int column, bool recursive)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | Indice di riga della cella specifica |
| colonna | Int32 | Indice di colonna della cella specifica. |
| ricorsivo | Booleano | Se restituisce quei dipendenti che non fanno riferimento direttamente alla cella specifica ma fanno riferimento ad altre foglie di quella cella. |

### Valore di ritorno

Enumeratore per enumerare tutti i dipendenti (oggetti Cell)

### Osservazioni

Per utilizzare questo metodo, assicurati che la cartella di lavoro sia impostata con valore true per [`EnableCalculationChain`](../../formulasettings/enablecalculationchain/) e sia stata completamente calcolata con questa impostazione. Se non esiste alcun riferimento di formula a questa cella, verrà restituito null. Per ulteriori dettagli ed esempi, consulta [`GetDependentsInCalculation`](../../cell/getdependentsincalculation/)

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellsMethodGetDependentsInCalculationWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e calcola le formule
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Configura le dipendenze delle formule:
            // C1 = 10 (valore di origine)
            // B1 = C1*2
            // A1 = B1+5
            cells["C1"].PutValue(10);
            cells["B1"].Formula = "C1*2";
            cells["A1"].Formula = "B1+5";

            // Calcola le formule per stabilire le dipendenze
            workbook.CalculateFormula();

            try
            {
                // Ottieni i dipendenti per la cella C1 (riga 0, colonna 2) con controllo ricorsivo
                IEnumerator dependents = cells.GetDependentsInCalculation(0, 2, true);

                Console.WriteLine("Dependents of cell C1:");
                while (dependents.MoveNext())
                {
                    if (dependents.Current is Cell dependentCell)
                    {
                        Console.WriteLine($"- {dependentCell.Name}");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetDependentsInCalculation: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("GetDependentsInCalculationDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


