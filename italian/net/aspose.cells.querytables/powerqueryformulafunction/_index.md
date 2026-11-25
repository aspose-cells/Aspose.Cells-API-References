---
title: "Classe PowerQueryFormulaFunction"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.QueryTables.PowerQueryFormulaFunction. Rappresenta la funzione di Power Query"
type: docs
url: /it/net/aspose.cells.querytables/powerqueryformulafunction/
---
## PowerQueryFormulaFunction class

Rappresenta la funzione di Power Query.

```csharp
public class PowerQueryFormulaFunction : PowerQueryFormula
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Description](../../aspose.cells.querytables/powerqueryformula/description/) { get; set; } | Ottiene e imposta la descrizione della formula power query.(Ereditato da [`PowerQueryFormula`](../powerqueryformula/).) |
| [F](../../aspose.cells.querytables/powerqueryformulafunction/f/) { get; set; } | Ottiene e imposta la definizione della funzione. |
| virtual [FormulaDefinition](../../aspose.cells.querytables/powerqueryformula/formuladefinition/) { get; } | Ottiene la definizione della formula Power Query.(Ereditato da [`PowerQueryFormula`](../powerqueryformula/).) |
| [GroupName](../../aspose.cells.querytables/powerqueryformula/groupname/) { get; } | Ottiene il nome del gruppo che contiene questa formula power query.(Ereditato da [`PowerQueryFormula`](../powerqueryformula/).) |
| [Name](../../aspose.cells.querytables/powerqueryformula/name/) { get; set; } | Ottiene e imposta il nome della formula power query.(Ereditato da [`PowerQueryFormula`](../powerqueryformula/).) |
| [PowerQueryFormulaItems](../../aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/) { get; } | Ottiene tutti gli elementi della formula power query.(Ereditato da [`PowerQueryFormula`](../powerqueryformula/).) |
| override [Type](../../aspose.cells.querytables/powerqueryformulafunction/type/) { get; } | Ottiene il tipo della formula power query. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class QueryTablesClassPowerQueryFormulaFunctionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook("source.xlsx");
            PowerQueryFormula formula = workbook.DataMashup.PowerQueryFormulas["from_timestamp"];
            
            Console.WriteLine($"Name: {formula.Name}");
            Console.WriteLine($"Type: {formula.Type}");
            
            PowerQueryFormulaFunction function = (PowerQueryFormulaFunction)formula;
            Console.WriteLine($"Signature: {function.F}");
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [PowerQueryFormula](../powerqueryformula/)
* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


