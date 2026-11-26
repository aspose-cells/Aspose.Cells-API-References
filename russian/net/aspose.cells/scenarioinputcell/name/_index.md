---
title: "ScenarioInputCell.Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ScenarioInputCell. Получает и задает адрес входной ячейки"
type: docs
url: /ru/net/aspose.cells/scenarioinputcell/name/
---
## ScenarioInputCell.Name property

Получает и задает адрес входной ячейки.

```csharp
public string Name { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать сценарий
            ScenarioCollection scenarios = worksheet.Scenarios;
            int scenarioIndex = scenarios.Add("TestScenario");

            // Получить сценарий
            Scenario scenario = scenarios[scenarioIndex];

            // Добавить входные ячейки в сценарий
            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(6, 15, "1"); // G16 is row 6, column 15 (0-based)
            inputCells.Add(7, 15, "2"); // H16 is row 7, column 15 (0-based)

            // Получить входные ячейки
            ScenarioInputCell inputCell1 = inputCells[0];
            ScenarioInputCell inputCell2 = inputCells[1];

            // Продемонстрировать использование свойства Name
            Console.WriteLine("First input cell name: " + inputCell1.Name);
            Console.WriteLine("Second input cell name: " + inputCell2.Name);

            // Проверить, что имена соответствуют ожидаемым значениям
            if (inputCell1.Name != "G16" || inputCell2.Name != "H16")
            {
                throw new Exception("Input cell names don't match expected values");
            }
        }
    }
}
```

### См. также

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


