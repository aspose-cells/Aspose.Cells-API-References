---
title: "ScenarioInputCellCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ScenarioInputCellCollection. Получает ScenarioInputCell по индексу в списке"
type: docs
url: /ru/net/aspose.cells/scenarioinputcellcollection/item/
---
## ScenarioInputCellCollection indexer

Получает [`ScenarioInputCell`](../../scenarioinputcell/) по индексу в списке.

```csharp
public ScenarioInputCell this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Конкретный индекс в списке |

### Возвращаемое значение

Объект [`ScenarioInputCell`](../../scenarioinputcell/)

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int scenarioIndex = worksheet.Scenarios.Add("Scenario1");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];
            ScenarioInputCellCollection inputCells = scenario.InputCells;

            inputCells.Add(0, 0, "10");
            inputCells.Add(1, 1, "20");

            // Продемонстрировать использование свойства Item
            ScenarioInputCell firstCell = inputCells[0];
            ScenarioInputCell secondCell = inputCells[1];

            Console.WriteLine($"First cell - Row: {firstCell.Row}, Column: {firstCell.Column}, Value: {firstCell.Value}");
            Console.WriteLine($"Second cell - Row: {secondCell.Row}, Column: {secondCell.Column}, Value: {secondCell.Value}");

            workbook.Save("ScenarioInputCellCollectionExample.xlsx");
        }
    }
}
```

### См. также

* class [ScenarioInputCell](../../scenarioinputcell/)
* class [ScenarioInputCellCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


