---
title: "Classe PowerQueryFormulaFunction"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.QueryTables.PowerQueryFormulaFunction. Représente la fonction de Power Query"
type: docs
url: /fr/net/aspose.cells.querytables/powerqueryformulafunction/
---
## PowerQueryFormulaFunction class

Représente la fonction de Power Query.

```csharp
public class PowerQueryFormulaFunction : PowerQueryFormula
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Description](../../aspose.cells.querytables/powerqueryformula/description/) { get; set; } | Obtient et définit la description de la formule Power Query.(Hérité de [`PowerQueryFormula`](../powerqueryformula/).) |
| [F](../../aspose.cells.querytables/powerqueryformulafunction/f/) { get; set; } | Obtient et définit la définition de la fonction. |
| virtual [FormulaDefinition](../../aspose.cells.querytables/powerqueryformula/formuladefinition/) { get; } | Obtient la définition de la formule Power Query.(Hérité de [`PowerQueryFormula`](../powerqueryformula/).) |
| [GroupName](../../aspose.cells.querytables/powerqueryformula/groupname/) { get; } | Obtient le nom du groupe qui contient cette formule Power Query.(Hérité de [`PowerQueryFormula`](../powerqueryformula/).) |
| [Name](../../aspose.cells.querytables/powerqueryformula/name/) { get; set; } | Obtient et définit le nom de la formule Power Query.(Hérité de [`PowerQueryFormula`](../powerqueryformula/).) |
| [PowerQueryFormulaItems](../../aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/) { get; } | Obtient tous les éléments de la formule Power Query.(Hérité de [`PowerQueryFormula`](../powerqueryformula/).) |
| override [Type](../../aspose.cells.querytables/powerqueryformulafunction/type/) { get; } | Obtient le type de la formule Power Query. |

### Exemples

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

### Voir aussi

* class [PowerQueryFormula](../powerqueryformula/)
* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


