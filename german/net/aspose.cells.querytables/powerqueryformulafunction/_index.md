---
title: "Klasse PowerQueryFormulaFunction"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.QueryTables.PowerQueryFormulaFunction class. Stellt die Funktion von Power Query dar"
type: docs
url: /de/net/aspose.cells.querytables/powerqueryformulafunction/
---
## PowerQueryFormulaFunction class

Stellt die Funktion von Power Query dar.

```csharp
public class PowerQueryFormulaFunction : PowerQueryFormula
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Description](../../aspose.cells.querytables/powerqueryformula/description/) { get; set; } | Liest und setzt die Beschreibung der Power‑Query‑Formel.(Geerbt von [`PowerQueryFormula`](../powerqueryformula/).) |
| [F](../../aspose.cells.querytables/powerqueryformulafunction/f/) { get; set; } | Liest und setzt die Definition der Funktion. |
| virtual [FormulaDefinition](../../aspose.cells.querytables/powerqueryformula/formuladefinition/) { get; } | Liest die Definition der Power Query-Formel. (Vererbt von [`PowerQueryFormula`](../powerqueryformula/).) |
| [GroupName](../../aspose.cells.querytables/powerqueryformula/groupname/) { get; } | Liest den Namen der Gruppe, die diese Power‑Query‑Formel enthält.(Geerbt von [`PowerQueryFormula`](../powerqueryformula/).) |
| [Name](../../aspose.cells.querytables/powerqueryformula/name/) { get; set; } | Liest und setzt den Namen der Power‑Query‑Formel.(Geerbt von [`PowerQueryFormula`](../powerqueryformula/).) |
| [PowerQueryFormulaItems](../../aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/) { get; } | Liest alle Elemente der Power‑Query‑Formel.(Geerbt von [`PowerQueryFormula`](../powerqueryformula/).) |
| override [Type](../../aspose.cells.querytables/powerqueryformulafunction/type/) { get; } | Liest den Typ der Power‑Query‑Formel. |

### Beispiele

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

### Siehe auch

* class [PowerQueryFormula](../powerqueryformula/)
* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


