---
title: "ScenarioInputCellCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ScenarioInputCellCollection. Добавляет входную ячейку"
type: docs
url: /ru/net/aspose.cells/scenarioinputcellcollection/add/
---
## ScenarioInputCellCollection.Add method

Добавляет ячейку ввода.

```csharp
public int Add(int row, int column, string value)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки входной ячейки. |
| column | Int32 | Индекс столбца входной ячейки. |
| значение | String | Значение входной ячейки. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellCollectionMethodAddWithInt32Int32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int scenarioIndex = worksheet.Scenarios.Add("TestScenario");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];
            ScenarioInputCellCollection inputCells = scenario.InputCells;

            inputCells.Add(0, 0, "10");
            inputCells.Add(1, 1, "20");

            Console.WriteLine($"Count: {inputCells.Count}");
            Console.WriteLine($"Cell 1: Row={inputCells[0].Row}, Column={inputCells[0].Column}, Value={inputCells[0].Value}");
            Console.WriteLine($"Cell 2: Row={inputCells[1].Row}, Column={inputCells[1].Column}, Value={inputCells[1].Value}");

            workbook.Save("ScenarioInputCellCollectionDemo.xlsx");
        }
    }
}
```

### См. также

* class [ScenarioInputCellCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


