---
title: "Klasse PowerQueryFormulaItemCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.QueryTables.PowerQueryFormulaItemCollection Klasse. Stellt alle Elemente der Power‑Query‑Formel dar"
type: docs
url: /de/net/aspose.cells.querytables/powerqueryformulaitemcollection/
---
## PowerQueryFormulaItemCollection class

Stellt alle Elemente der Power‑Query‑Formel dar.

```csharp
public class PowerQueryFormulaItemCollection : CollectionBase<PowerQueryFormulaItem>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.querytables/powerqueryformulaitemcollection/item/) { get; } | Liest [`PowerQueryFormulaItem`](../powerqueryformulaitem/) anhand des Index in der Liste. (2 Indexer) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PowerQueryFormulaItem) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PowerQueryFormulaItem, IComparer&lt;PowerQueryFormulaItem&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, PowerQueryFormulaItem, IComparer&lt;PowerQueryFormulaItem&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(PowerQueryFormulaItem) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PowerQueryFormulaItem[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PowerQueryFormulaItem[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, PowerQueryFormulaItem[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;PowerQueryFormulaItem&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;PowerQueryFormulaItem&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;PowerQueryFormulaItem&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;PowerQueryFormulaItem&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;PowerQueryFormulaItem&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;PowerQueryFormulaItem&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;PowerQueryFormulaItem&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;PowerQueryFormulaItem&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;PowerQueryFormulaItem&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;PowerQueryFormulaItem&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PowerQueryFormulaItem) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PowerQueryFormulaItem, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PowerQueryFormulaItem, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PowerQueryFormulaItem) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PowerQueryFormulaItem, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PowerQueryFormulaItem, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class QueryTablesClassPowerQueryFormulaItemCollectionDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für Power Query hinzu (simuliert, da wir keine echten PQ‑Formeln programmgesteuert erstellen können)
            // Normalerweise würden Sie eine vorhandene Datei mit PQ‑Formeln laden
            string sourcePath = "example.xlsm";
            try
            {
                workbook = new Workbook(sourcePath);
            }
            catch
            {
                Console.WriteLine("File not found. Using new workbook for demonstration.");
                return;
            }

            // Greife auf Power Query‑Formeln zu
            PowerQueryFormulaCollection pqFormulas = workbook.DataMashup.PowerQueryFormulas;
            
            if (pqFormulas.Count > 0)
            {
                // Hole die erste Power Query‑Formel
                PowerQueryFormula formula = pqFormulas[0];
                Console.WriteLine("Formula Name: {0}", formula.Name);

                // Greife auf Formelelemente zu
                PowerQueryFormulaItemCollection items = formula.PowerQueryFormulaItems;
                Console.WriteLine("Number of items: {0}", items.Count);

                if (items.Count > 0)
                {
                    // Zeige das erste Element an
                    PowerQueryFormulaItem item = items[0];
                    Console.WriteLine("Item Name: {0}", item.Name);
                    Console.WriteLine("Item Value: {0}", item.Value);
                }
            }
            else
            {
                Console.WriteLine("No Power Query formulas found in the workbook.");
            }
        }
    }
}
```

### Siehe auch

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [PowerQueryFormulaItem](../powerqueryformulaitem/)
* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


