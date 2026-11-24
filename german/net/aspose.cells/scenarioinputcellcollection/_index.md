---
title: "Klasse ScenarioInputCellCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ScenarioInputCellCollection Klasse. Stellt die Liste der Eingabezellen der Szenarien dar"
type: docs
url: /de/net/aspose.cells/scenarioinputcellcollection/
---
## ScenarioInputCellCollection class

Stellt die Liste der Eingabezellen des Szenarios dar.

```csharp
public class ScenarioInputCellCollection : CollectionBase<ScenarioInputCell>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/scenarioinputcellcollection/item/) { get; } | Liefert [`ScenarioInputCell`](../scenarioinputcell/) nach Index in der Liste. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells/scenarioinputcellcollection/add/)(int, int, string) | Fügt eine Eingabezelle hinzu. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ScenarioInputCell) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ScenarioInputCell, IComparer&lt;ScenarioInputCell&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ScenarioInputCell, IComparer&lt;ScenarioInputCell&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ScenarioInputCell) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ScenarioInputCell[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ScenarioInputCell[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ScenarioInputCell[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ScenarioInputCell&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ScenarioInputCell&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ScenarioInputCell&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ScenarioInputCell&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ScenarioInputCell&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ScenarioInputCell&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ScenarioInputCell&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ScenarioInputCell&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ScenarioInputCell&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ScenarioInputCell&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ScenarioInputCell) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ScenarioInputCell, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ScenarioInputCell, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ScenarioInputCell) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ScenarioInputCell, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ScenarioInputCell, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ScenarioInputCellCollectionDemo
    {
        public static void ScenarioInputCellCollectionExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Szenario dem Arbeitsblatt hinzu.
            int scenarioIndex = worksheet.Scenarios.Add("Scenario1");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Greife auf die ScenarioInputCellCollection zu
            ScenarioInputCellCollection inputCells = scenario.InputCells;

            // Füge Eingabezellen dem Szenario hinzu.
            inputCells.Add(0, 0, "10"); // Adding cell A1 with value 10
            inputCells.Add(1, 1, "20"); // Adding cell B2 with value 20

            // Greife zu und drucke die Eigenschaften der ScenarioInputCellCollection
            Console.WriteLine("Capacity: " + inputCells.Capacity);
            Console.WriteLine("Count: " + inputCells.Count);

            // Greife auf einzelne ScenarioInputCell per Index zu
            ScenarioInputCell inputCell1 = inputCells[0];
            ScenarioInputCell inputCell2 = inputCells[1];

            // Drucke Details der Eingabezellen
            Console.WriteLine($"Input Cell 1: Row={inputCell1.Row}, Column={inputCell1.Column}, Value={inputCell1.Value}");
            Console.WriteLine($"Input Cell 2: Row={inputCell2.Row}, Column={inputCell2.Column}, Value={inputCell2.Value}");

            // Speichere die Arbeitsmappe
            workbook.Save("ScenarioInputCellCollectionExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [ScenarioInputCell](../scenarioinputcell/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


