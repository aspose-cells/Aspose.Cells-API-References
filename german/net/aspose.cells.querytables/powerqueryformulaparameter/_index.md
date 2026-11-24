---
title: "Klasse PowerQueryFormulaParameter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.QueryTables.PowerQueryFormulaParameter Klasse. Stellt den Parameter der Power‑Query‑Formel dar"
type: docs
url: /de/net/aspose.cells.querytables/powerqueryformulaparameter/
---
## PowerQueryFormulaParameter class

Stellt den Parameter der Power‑Query‑Formel dar.

```csharp
public class PowerQueryFormulaParameter : PowerQueryFormula
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Description](../../aspose.cells.querytables/powerqueryformula/description/) { get; set; } | Liest und setzt die Beschreibung der Power‑Query‑Formel.(Geerbt von [`PowerQueryFormula`](../powerqueryformula/).) |
| override [FormulaDefinition](../../aspose.cells.querytables/powerqueryformulaparameter/formuladefinition/) { get; } | Liest die Definition des Parameters. |
| [GroupName](../../aspose.cells.querytables/powerqueryformula/groupname/) { get; } | Liest den Namen der Gruppe, die diese Power‑Query‑Formel enthält.(Geerbt von [`PowerQueryFormula`](../powerqueryformula/).) |
| [Name](../../aspose.cells.querytables/powerqueryformula/name/) { get; set; } | Liest und setzt den Namen der Power‑Query‑Formel.(Geerbt von [`PowerQueryFormula`](../powerqueryformula/).) |
| [ParameterDefinition](../../aspose.cells.querytables/powerqueryformulaparameter/parameterdefinition/) { get; } | (**Obsolet.**) Liest die Definition des Parameters. |
| [PowerQueryFormulaItems](../../aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/) { get; } | Liest alle Elemente der Power‑Query‑Formel.(Geerbt von [`PowerQueryFormula`](../powerqueryformula/).) |
| override [Type](../../aspose.cells.querytables/powerqueryformulaparameter/type/) { get; } | Liest den Typ der Power‑Query‑Formel. |
| [Value](../../aspose.cells.querytables/powerqueryformulaparameter/value/) { get; set; } | Liest den Wert des Parameters. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook("PowerQueryFormulaDemo_original.xlsx");

            // Greift auf die DataMashup‑Eigenschaft der Arbeitsmappe zu
            DataMashup dataMashup = workbook.DataMashup;

            if (dataMashup != null)
            {
                // Greift auf die PowerQueryFormulas‑Eigenschaft zu
                PowerQueryFormulaCollection powerQueryFormulas = dataMashup.PowerQueryFormulas;

                // Greift auf die PowerQueryFormulaParameters‑Eigenschaft zu
                PowerQueryFormulaParameterCollection powerQueryFormulaParameters = dataMashup.PowerQueryFormulaParameters;

                // Beispielhafte Verwendung: Durchlaufen von PowerQueryFormulas
                foreach (PowerQueryFormula formula in powerQueryFormulas)
                {
                    Console.WriteLine(formula.Name);
                }

                // Beispielhafte Verwendung: Durchlaufen von PowerQueryFormulaParameters
                foreach (PowerQueryFormulaParameter para in powerQueryFormulaParameters)
                {
                    // Zeige die Parameterdetails an
                    Console.WriteLine("Parameter Name: " + para.Name);
                    Console.WriteLine("Parameter Value: " + para.Value);

                    Console.WriteLine("Parameter Definition: " + para.ParameterDefinition);
                }
            }
            

            // Speichere die Arbeitsmappe
            workbook.Save("PowerQueryFormulaParameterExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* class [PowerQueryFormula](../powerqueryformula/)
* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


