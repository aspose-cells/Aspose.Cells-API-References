---
title: "Класс ScenarioCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.ScenarioCollection. Представляет список сценариев"
type: docs
url: /ru/net/aspose.cells/scenariocollection/
---
## ScenarioCollection class

Представляет список сценариев.

```csharp
public class ScenarioCollection : CollectionBase<Scenario>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [ActiveIndex](../../aspose.cells/scenariocollection/activeindex/) { get; set; } | Получает и задает, какой сценарий выбран. |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/scenariocollection/item/) { get; } | Получает объект [`Scenario`](../scenario/) по индексу. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [LastSelected](../../aspose.cells/scenariocollection/lastselected/) { get; set; } | Указывает, какой сценарий был последним выбран пользователем для выполнения/отображения. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells/scenariocollection/add/)(string) | Добавляет сценарий. |
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

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ScenarioCollectionDemo
    {
        public static void ScenarioCollectionExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить доступ к ScenarioCollection рабочего листа
            ScenarioCollection scenarios = worksheet.Scenarios;

            // Добавить новый сценарий в коллекцию.
            int scenarioIndex = scenarios.Add("Scenario1");

            // Получить доступ к только что добавленному сценарию.
            Scenario scenario = scenarios[scenarioIndex];

            // Установить некоторые свойства для сценария.
            scenario.Comment = "This is a test scenario.";
            scenario.IsHidden = false;

            // Установить индекс активного сценария.
            scenarios.ActiveIndex = scenarioIndex;

            // Установить индекс последнего выбранного сценария.
            scenarios.LastSelected = scenarioIndex;

            // Сохраните книгу
            workbook.Save("ScenarioCollectionExample.xlsx");

            return;
        }
    }
}
```

### См. также

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Scenario](../scenario/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


