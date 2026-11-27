---
title: "Klass PowerQueryFormulaParameter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.QueryTables.PowerQueryFormulaParameter klass. Representerar parametern för power query-formeln"
type: docs
url: /sv/net/aspose.cells.querytables/powerqueryformulaparameter/
---
## PowerQueryFormulaParameter class

Representerar parametern för Power Query‑formeln.

```csharp
public class PowerQueryFormulaParameter : PowerQueryFormula
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Description](../../aspose.cells.querytables/powerqueryformula/description/) { get; set; } | Hämtar och anger beskrivningen av power query-formeln.(Ärvd från [`PowerQueryFormula`](../powerqueryformula/).) |
| override [FormulaDefinition](../../aspose.cells.querytables/powerqueryformulaparameter/formuladefinition/) { get; } | Hämtar definitionen av parametern. |
| [GroupName](../../aspose.cells.querytables/powerqueryformula/groupname/) { get; } | Hämtar namnet på gruppen som innehåller denna power query-formel.(Ärvd från [`PowerQueryFormula`](../powerqueryformula/).) |
| [Name](../../aspose.cells.querytables/powerqueryformula/name/) { get; set; } | Hämtar och anger namnet på power query-formeln.(Ärvd från [`PowerQueryFormula`](../powerqueryformula/).) |
| [ParameterDefinition](../../aspose.cells.querytables/powerqueryformulaparameter/parameterdefinition/) { get; } | (**Föråldrad.**) Hämtar definitionen av parametern. |
| [PowerQueryFormulaItems](../../aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/) { get; } | Hämtar alla objekt av power query-formeln.(Ärvd från [`PowerQueryFormula`](../powerqueryformula/).) |
| override [Type](../../aspose.cells.querytables/powerqueryformulaparameter/type/) { get; } | Hämtar typen av power query-formeln. |
| [Value](../../aspose.cells.querytables/powerqueryformulaparameter/value/) { get; set; } | Hämtar värdet av parametern. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaParameterDemo
    {
        public static void PowerQueryFormulaParameterExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook("PowerQueryFormulaDemo_original.xlsx");

            // Åtkomst till DataMashup-egenskapen i arbetsboken
            DataMashup dataMashup = workbook.DataMashup;

            if (dataMashup != null)
            {
                // Åtkomst till PowerQueryFormulas-egenskapen
                PowerQueryFormulaCollection powerQueryFormulas = dataMashup.PowerQueryFormulas;

                // Åtkomst till PowerQueryFormulaParameters-egenskapen
                PowerQueryFormulaParameterCollection powerQueryFormulaParameters = dataMashup.PowerQueryFormulaParameters;

                // Exempel på användning: Iterera genom PowerQueryFormulas
                foreach (PowerQueryFormula formula in powerQueryFormulas)
                {
                    Console.WriteLine(formula.Name);
                }

                // Exempel på användning: Iterera genom PowerQueryFormulaParameters
                foreach (PowerQueryFormulaParameter para in powerQueryFormulaParameters)
                {
                    // Visa parameterdetaljerna
                    Console.WriteLine("Parameter Name: " + para.Name);
                    Console.WriteLine("Parameter Value: " + para.Value);

                    Console.WriteLine("Parameter Definition: " + para.ParameterDefinition);
                }
            }
            

            // Spara arbetsboken
            workbook.Save("PowerQueryFormulaParameterExample.xlsx");

            return;
        }
    }
}
```

### Se även

* class [PowerQueryFormula](../powerqueryformula/)
* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


