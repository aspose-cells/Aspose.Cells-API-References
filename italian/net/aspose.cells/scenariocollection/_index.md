---
title: "Classe ScenarioCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.ScenarioCollection. Rappresenta l'elenco degli scenari"
type: docs
url: /it/net/aspose.cells/scenariocollection/
---
## ScenarioCollection class

Rappresenta l'elenco degli scenari.

```csharp
public class ScenarioCollection : CollectionBase<Scenario>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ActiveIndex](../../aspose.cells/scenariocollection/activeindex/) { get; set; } | Ottiene e imposta quale scenario è selezionato. |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/scenariocollection/item/) { get; } | Ottiene l'oggetto [`Scenario`](../scenario/) per indice. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [LastSelected](../../aspose.cells/scenariocollection/lastselected/) { get; set; } | Indica quale scenario è stato selezionato per ultimo dall'utente per essere eseguito/visualizzato. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells/scenariocollection/add/)(string) | Aggiunge uno scenario. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Scenario) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Scenario, IComparer&lt;Scenario&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Scenario, IComparer&lt;Scenario&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Scenario) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Scenario[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Scenario[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Scenario[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Scenario&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Scenario&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Scenario&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Scenario&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Scenario&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Scenario&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Scenario&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Scenario&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Scenario&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Scenario&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Scenario) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Scenario, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Scenario, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Scenario) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Scenario, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Scenario, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ScenarioCollectionDemo
    {
        public static void ScenarioCollectionExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi alla ScenarioCollection del foglio di lavoro
            ScenarioCollection scenarios = worksheet.Scenarios;

            // Aggiungi un nuovo scenario alla collezione
            int scenarioIndex = scenarios.Add("Scenario1");

            // Accedi allo scenario appena aggiunto
            Scenario scenario = scenarios[scenarioIndex];

            // Imposta alcune proprietà per lo scenario
            scenario.Comment = "This is a test scenario.";
            scenario.IsHidden = false;

            // Imposta l'indice dello scenario attivo
            scenarios.ActiveIndex = scenarioIndex;

            // Imposta l'indice dell'ultimo scenario selezionato
            scenarios.LastSelected = scenarioIndex;

            // Salva la cartella di lavoro
            workbook.Save("ScenarioCollectionExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Scenario](../scenario/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


