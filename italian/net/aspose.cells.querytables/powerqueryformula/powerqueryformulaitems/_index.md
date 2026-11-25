---
title: "PowerQueryFormula.PowerQueryFormulaItems"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PowerQueryFormula. Ottiene tutti gli elementi della formula Power Query"
type: docs
url: /it/net/aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/
---
## PowerQueryFormula.PowerQueryFormulaItems property

Ottiene tutti gli elementi della formula Power Query.

```csharp
public PowerQueryFormulaItemCollection PowerQueryFormulaItems { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaPropertyPowerQueryFormulaItemsDemo
    {
        public static void Run()
        {
            // Carica la cartella di lavoro di origine
            Workbook workbook = new Workbook("example.xlsx");

            // Accedi alla prima formula Power Query e al suo primo elemento
            PowerQueryFormulaItem item = workbook.DataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0];
            
            // Modifica il valore dell'elemento (sostituisci la lettera dell'unità)
            string modifiedValue = item.Value.Replace(@"C:\", @"D:\");
            item.Value = modifiedValue;

            // Salva la cartella di lavoro
            workbook.Save("modified_example.xlsx");

            // Verifica la modifica
            Console.WriteLine("Original value modified to: " + modifiedValue);
        }
    }
}
```

### Vedi anche

* class [PowerQueryFormulaItemCollection](../../powerqueryformulaitemcollection/)
* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


