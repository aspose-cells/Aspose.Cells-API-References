---
title: "Klass PowerQueryFormulaFunction"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.QueryTables.PowerQueryFormulaFunction‑klass. Representerar funktionen i Power Query."
type: docs
url: /sv/net/aspose.cells.querytables/powerqueryformulafunction/
---
## PowerQueryFormulaFunction class

Representerar funktionen för Power Query.

```csharp
public class PowerQueryFormulaFunction : PowerQueryFormula
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Description](../../aspose.cells.querytables/powerqueryformula/description/) { get; set; } | Hämtar och anger beskrivningen av power query-formeln.(Ärvd från [`PowerQueryFormula`](../powerqueryformula/).) |
| [F](../../aspose.cells.querytables/powerqueryformulafunction/f/) { get; set; } | Hämtar och anger definitionen av funktionen. |
| virtual [FormulaDefinition](../../aspose.cells.querytables/powerqueryformula/formuladefinition/) { get; } | Hämtar definitionen av Power Query‑formeln.(Ärvd från [`PowerQueryFormula`](../powerqueryformula/).) |
| [GroupName](../../aspose.cells.querytables/powerqueryformula/groupname/) { get; } | Hämtar namnet på gruppen som innehåller denna power query-formel.(Ärvd från [`PowerQueryFormula`](../powerqueryformula/).) |
| [Name](../../aspose.cells.querytables/powerqueryformula/name/) { get; set; } | Hämtar och anger namnet på power query-formeln.(Ärvd från [`PowerQueryFormula`](../powerqueryformula/).) |
| [PowerQueryFormulaItems](../../aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/) { get; } | Hämtar alla objekt av power query-formeln.(Ärvd från [`PowerQueryFormula`](../powerqueryformula/).) |
| override [Type](../../aspose.cells.querytables/powerqueryformulafunction/type/) { get; } | Hämtar typen av power query-formeln. |

### Exempel

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

### Se även

* class [PowerQueryFormula](../powerqueryformula/)
* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


