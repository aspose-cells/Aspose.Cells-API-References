---
title: "Classe PowerQueryFormulaParameter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.QueryTables.PowerQueryFormulaParameter classe. Rappresenta il parametro della formula power query"
type: docs
url: /it/net/aspose.cells.querytables/powerqueryformulaparameter/
---
## PowerQueryFormulaParameter class

Rappresenta il parametro della formula Power Query.

```csharp
public class PowerQueryFormulaParameter : PowerQueryFormula
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Description](../../aspose.cells.querytables/powerqueryformula/description/) { get; set; } | Ottiene e imposta la descrizione della formula power query.(Ereditato da [`PowerQueryFormula`](../powerqueryformula/).) |
| override [FormulaDefinition](../../aspose.cells.querytables/powerqueryformulaparameter/formuladefinition/) { get; } | Ottiene la definizione del parametro. |
| [GroupName](../../aspose.cells.querytables/powerqueryformula/groupname/) { get; } | Ottiene il nome del gruppo che contiene questa formula power query.(Ereditato da [`PowerQueryFormula`](../powerqueryformula/).) |
| [Name](../../aspose.cells.querytables/powerqueryformula/name/) { get; set; } | Ottiene e imposta il nome della formula power query.(Ereditato da [`PowerQueryFormula`](../powerqueryformula/).) |
| [ParameterDefinition](../../aspose.cells.querytables/powerqueryformulaparameter/parameterdefinition/) { get; } | (**Obsoleto.**) Ottiene la definizione del parametro. |
| [PowerQueryFormulaItems](../../aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/) { get; } | Ottiene tutti gli elementi della formula power query.(Ereditato da [`PowerQueryFormula`](../powerqueryformula/).) |
| override [Type](../../aspose.cells.querytables/powerqueryformulaparameter/type/) { get; } | Ottiene il tipo della formula power query. |
| [Value](../../aspose.cells.querytables/powerqueryformulaparameter/value/) { get; set; } | Ottiene il valore del parametro. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook("PowerQueryFormulaDemo_original.xlsx");

            // Accedi alla proprietà DataMashup della cartella di lavoro
            DataMashup dataMashup = workbook.DataMashup;

            if (dataMashup != null)
            {
                // Accedi alla proprietà PowerQueryFormulas
                PowerQueryFormulaCollection powerQueryFormulas = dataMashup.PowerQueryFormulas;

                // Accedi alla proprietà PowerQueryFormulaParameters
                PowerQueryFormulaParameterCollection powerQueryFormulaParameters = dataMashup.PowerQueryFormulaParameters;

                // Esempio di utilizzo: iterare attraverso PowerQueryFormulas
                foreach (PowerQueryFormula formula in powerQueryFormulas)
                {
                    Console.WriteLine(formula.Name);
                }

                // Esempio di utilizzo: iterare attraverso PowerQueryFormulaParameters
                foreach (PowerQueryFormulaParameter para in powerQueryFormulaParameters)
                {
                    // Visualizza i dettagli del parametro
                    Console.WriteLine("Parameter Name: " + para.Name);
                    Console.WriteLine("Parameter Value: " + para.Value);

                    Console.WriteLine("Parameter Definition: " + para.ParameterDefinition);
                }
            }
            

            // Salva la cartella di lavoro
            workbook.Save("PowerQueryFormulaParameterExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* class [PowerQueryFormula](../powerqueryformula/)
* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


