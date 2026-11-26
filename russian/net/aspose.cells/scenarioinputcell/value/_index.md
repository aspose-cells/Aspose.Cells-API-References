---
title: "ScenarioInputCell.Value"
second_title: "Справочник API Aspose.Cells для .NET"
description: "ScenarioInputCell свойство. Получает и задаёт значение входной ячейки"
type: docs
url: /ru/net/aspose.cells/scenarioinputcell/value/
---
## ScenarioInputCell.Value property

Получает и задает значение входной ячейки.

```csharp
public string Value { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить сценарий
            int scenarioIndex = worksheet.Scenarios.Add("TestScenario");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Добавить входные ячейки со значениями
            scenario.InputCells.Add(0, 0, "100"); // Cell A1
            scenario.InputCells.Add(1, 1, "200"); // Cell B2

            // Получать и изменять значения
            ScenarioInputCell cell1 = scenario.InputCells[0];
            Console.WriteLine($"Original value: {cell1.Value}");
            cell1.Value = "150"; // Modify the value
            Console.WriteLine($"Modified value: {cell1.Value}");

            // Сохраните книгу
            workbook.Save("ScenarioValueDemo.xlsx");
        }
    }
}
```

### См. также

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


