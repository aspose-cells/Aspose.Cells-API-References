---
title: "PowerQueryFormulaFunction.F"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PowerQueryFormulaFunction. Ottiene e imposta la definizione della funzione"
type: docs
url: /it/net/aspose.cells.querytables/powerqueryformulafunction/f/
---
## PowerQueryFormulaFunction.F property

Ottiene e imposta la definizione della funzione.

```csharp
public string F { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaFunctionPropertyFDemo
    {
        public static void Run()
        {
            // Carica un workbook che contiene formule Power Query esistenti
            Workbook workbook = new Workbook("example.xlsx");
            
            // Accedi alla raccolta di formule Power Query
            PowerQueryFormulaCollection queryFormulas = workbook.DataMashup.PowerQueryFormulas;
            
            // Recupera una formula di funzione esistente per nome
            PowerQueryFormula formula = queryFormulas["from_timestamp"];
            
            // Esegui il cast a PowerQueryFormulaFunction per accedere alla proprietà F
            if (formula is PowerQueryFormulaFunction function)
            {
                // Dimostrare il recupero della proprietà F
                Console.WriteLine("Original Function Definition: " + function.F);
                
                // Dimostrare l'impostazione della proprietà F
                function.F = "(x as number) as datetimezone => #datetimezone(1970,1,1,0,0,0,0,0) + #duration(0,0,0,x)";
                Console.WriteLine("Updated Function Definition: " + function.F);
            }
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [PowerQueryFormulaFunction](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


