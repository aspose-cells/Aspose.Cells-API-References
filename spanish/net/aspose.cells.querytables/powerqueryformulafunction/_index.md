---
title: "Clase PowerQueryFormulaFunction"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.QueryTables.PowerQueryFormulaFunction. Representa la función de Power Query"
type: docs
url: /es/net/aspose.cells.querytables/powerqueryformulafunction/
---
## PowerQueryFormulaFunction class

Representa la función de Power Query.

```csharp
public class PowerQueryFormulaFunction : PowerQueryFormula
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Description](../../aspose.cells.querytables/powerqueryformula/description/) { get; set; } | Obtiene y establece la descripción de la fórmula de Power Query.(Heredado de [`PowerQueryFormula`](../powerqueryformula/).) |
| [F](../../aspose.cells.querytables/powerqueryformulafunction/f/) { get; set; } | Obtiene y establece la definición de la función. |
| virtual [FormulaDefinition](../../aspose.cells.querytables/powerqueryformula/formuladefinition/) { get; } | Obtiene la definición de la fórmula de Power Query. (Hereda de [`PowerQueryFormula`](../powerqueryformula/).) |
| [GroupName](../../aspose.cells.querytables/powerqueryformula/groupname/) { get; } | Obtiene el nombre del grupo que contiene esta fórmula de Power Query.(Heredado de [`PowerQueryFormula`](../powerqueryformula/).) |
| [Name](../../aspose.cells.querytables/powerqueryformula/name/) { get; set; } | Obtiene y establece el nombre de la fórmula de Power Query.(Heredado de [`PowerQueryFormula`](../powerqueryformula/).) |
| [PowerQueryFormulaItems](../../aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/) { get; } | Obtiene todos los elementos de la fórmula de Power Query.(Heredado de [`PowerQueryFormula`](../powerqueryformula/).) |
| override [Type](../../aspose.cells.querytables/powerqueryformulafunction/type/) { get; } | Obtiene el tipo de la fórmula de Power Query. |

### Ejemplos

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

### Ver también

* class [PowerQueryFormula](../powerqueryformula/)
* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


