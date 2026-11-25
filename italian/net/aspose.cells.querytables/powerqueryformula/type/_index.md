---
title: "PowerQueryFormula.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PowerQueryFormula. Ottiene il tipo di questa formula Power Query"
type: docs
url: /it/net/aspose.cells.querytables/powerqueryformula/type/
---
## PowerQueryFormula.Type property

Ottiene il tipo di questa formula Power Query.

```csharp
public virtual PowerQueryFormulaType Type { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Recupera le formule esistenti (nessuna nella nuova cartella di lavoro) per dimostrare la proprietà Type
            var formulas = workbook.DataMashup.PowerQueryFormulas;
            
            // In uno scenario reale con formule esistenti, controlleremmo i loro tipi
            Console.WriteLine("Power Query Formula Types:");
            
            // Questo dimostra il controllo della proprietà Type
            foreach (PowerQueryFormula formula in formulas)
            {
                Console.WriteLine($"- {formula.Name}: {formula.Type}");
            }

            // Per scopi dimostrativi, aggiungi output quando non esistono formule
            if (formulas.Count == 0)
            {
                Console.WriteLine("No power query formulas found in the workbook.");
                Console.WriteLine("Example formula types would be:");
                Console.WriteLine("- Function: " + PowerQueryFormulaType.Function);
                Console.WriteLine("- Parameter: " + PowerQueryFormulaType.Parameter);
                Console.WriteLine("- Formula: " + PowerQueryFormulaType.Formula);
            }

            // Salva la cartella di lavoro
            workbook.Save("PowerQueryFormulaTypes.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PowerQueryFormulaType](../../powerqueryformulatype/)
* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


