---
title: "Classe PowerQueryFormulaCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.QueryTables.PowerQueryFormulaCollection. Rappresenta tutte le formule Power Query nei dati mashup"
type: docs
url: /it/net/aspose.cells.querytables/powerqueryformulacollection/
---
## PowerQueryFormulaCollection class

Rappresenta tutte le formule Power Query nei dati mashup.

```csharp
public class PowerQueryFormulaCollection : CollectionBase<PowerQueryFormula>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.querytables/powerqueryformulacollection/item/) { get; } | Ottiene [`PowerQueryFormula`](../powerqueryformula/) per indice nella lista. (2 indicizzatori) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PowerQueryFormula) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PowerQueryFormula, IComparer&lt;PowerQueryFormula&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, PowerQueryFormula, IComparer&lt;PowerQueryFormula&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(PowerQueryFormula) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PowerQueryFormula[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PowerQueryFormula[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, PowerQueryFormula[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;PowerQueryFormula&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;PowerQueryFormula&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;PowerQueryFormula&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;PowerQueryFormula&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;PowerQueryFormula&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;PowerQueryFormula&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;PowerQueryFormula&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;PowerQueryFormula&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;PowerQueryFormula&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;PowerQueryFormula&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PowerQueryFormula) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PowerQueryFormula, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PowerQueryFormula, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PowerQueryFormula) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PowerQueryFormula, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PowerQueryFormula, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
| [RemoveBy](../../aspose.cells.querytables/powerqueryformulacollection/removeby/)(string) | Rimuove la formula Power Query per nome. |

### Esempi

```csharp
using Aspose.Cells;
using Aspose.Cells.QueryTables;
using System;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaDemo
    {
        public static void RunDemo()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook("PowerQueryFormulaDemo_original.xlsx");

            // Crea un oggetto DataMashup
            DataMashup dataMashup = workbook.DataMashup;

            // Accedi alla raccolta PowerQueryFormulas
            PowerQueryFormulaCollection powerQueryFormulas = dataMashup.PowerQueryFormulas;

            // Visualizza il conteggio delle formule Power Query
            Console.WriteLine($"Number of Power Query Formulas: {powerQueryFormulas.Count}");

            // Esempio di accesso a una specifica formula Power Query (se esistente)
            if (powerQueryFormulas.Count > 0)
            {
                PowerQueryFormula firstFormula = powerQueryFormulas[0];
                Console.WriteLine($"First Power Query Formula: {firstFormula}");
            }

            // Salva la cartella di lavoro
            workbook.Save("PowerQueryFormulaDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [PowerQueryFormula](../powerqueryformula/)
* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


