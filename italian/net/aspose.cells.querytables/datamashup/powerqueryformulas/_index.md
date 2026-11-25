---
title: "DataMashup.PowerQueryFormulas"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataMashup. Restituisce tutte le formule Power Query"
type: docs
url: /it/net/aspose.cells.querytables/datamashup/powerqueryformulas/
---
## DataMashup.PowerQueryFormulas property

Ottiene tutte le formule Power Query.

```csharp
public PowerQueryFormulaCollection PowerQueryFormulas { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class DataMashupPropertyPowerQueryFormulasDemo
    {
        public static void Run()
        {
            // Carica la cartella di lavoro con le formule Power Query
            Workbook workbook = new Workbook("source.xlsx");
            
            // Ottieni l'oggetto DataMashup
            DataMashup mashupData = workbook.DataMashup;
            
            // Verifica se ci sono formule Power Query
            if (mashupData != null && mashupData.PowerQueryFormulas != null)
            {
                Console.WriteLine("Power Query Formulas Found:");
                
                // Itera attraverso ogni formula Power Query
                foreach (PowerQueryFormula formula in mashupData.PowerQueryFormulas)
                {
                    Console.WriteLine("Formula Definition:");
                    Console.WriteLine(formula.FormulaDefinition);
                    Console.WriteLine("----------------------");
                }
            }
            else
            {
                Console.WriteLine("No Power Query formulas found in the workbook.");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [PowerQueryFormulaCollection](../../powerqueryformulacollection/)
* class [DataMashup](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


