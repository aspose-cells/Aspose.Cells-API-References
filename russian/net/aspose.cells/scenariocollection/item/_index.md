---
title: "ScenarioCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ScenarioCollection. Получает объект Scenario по индексу"
type: docs
url: /ru/net/aspose.cells/scenariocollection/item/
---
## ScenarioCollection indexer

Получает объект [`Scenario`](../../scenario/) по индексу.

```csharp
public Scenario this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Конкретный индекс в списке. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int scenarioIndex = worksheet.Scenarios.Add("TestScenario");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            scenario.InputCells.Add(0, 0, "100");
            scenario.InputCells.Add(1, 1, "200");

            // Продемонстрировать использование свойства Item
            ScenarioInputCell firstCell = scenario.InputCells[0];
            Console.WriteLine($"First cell - Row: {firstCell.Row}, Column: {firstCell.Column}, Value: {firstCell.Value}");

            workbook.Save("ScenarioCollectionDemo.xlsx");
        }
    }
}
```

### См. также

* class [Scenario](../../scenario/)
* class [ScenarioCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


