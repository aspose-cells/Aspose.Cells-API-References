---
title: "PowerQueryFormula.Name"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PowerQueryFormula. Ottiene e imposta il nome della formula Power Query"
type: docs
url: /it/net/aspose.cells.querytables/powerqueryformula/name/
---
## PowerQueryFormula.Name property

Ottiene e imposta il nome della formula Power Query.

```csharp
public string Name { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaPropertyNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Carica un file esistente con formule Power Query
            workbook = new Workbook("example.xlsx");
            
            // Accedi alle formule Power Query esistenti
            if (workbook.DataMashup.PowerQueryFormulas.Count > 0)
            {
                PowerQueryFormula formula = workbook.DataMashup.PowerQueryFormulas[0];
                
                // Dimostra l'uso della proprietà Name
                Console.WriteLine("Original Power Query Formula Name: " + formula.Name);
                
                // Modifica il nome
                formula.Name = "UpdatedSalesFilter";
                Console.WriteLine("Updated Power Query Formula Name: " + formula.Name);
                
                // Salva la cartella di lavoro
                workbook.Save("PowerQueryFormulaDemo.xlsx");
            }
            else
            {
                Console.WriteLine("No Power Query formulas found in the workbook.");
            }
        }
    }
}
```

### Vedi anche

* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


