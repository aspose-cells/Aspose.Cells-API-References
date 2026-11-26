---
title: "ScenarioInputCell.Column"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ScenarioInputCell. Получает и задает индекс столбца входной ячейки"
type: docs
url: /ru/net/aspose.cells/scenarioinputcell/column/
---
## ScenarioInputCell.Column property

Получает и задает индекс столбца входной ячейки.

```csharp
public int Column { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyColumnDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить сценарий в рабочий лист
            int scenarioIndex = worksheet.Scenarios.Add("Scenario1");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Добавить входные ячейки в сценарий
            scenario.InputCells.Add(0, 0, "10"); // Cell A1
            scenario.InputCells.Add(1, 1, "20"); // Cell B2

            // Получить доступ и продемонстрировать свойство Column
            ScenarioInputCell cell1 = scenario.InputCells[0];
            Console.WriteLine($"First input cell is at column: {cell1.Column}");

            // Поскольку Column только для чтения, нам нужно удалить и добавить заново, чтобы изменить столбец
            string value = cell1.Value;
            scenario.InputCells.RemoveAt(0);
            scenario.InputCells.Add(0, 2, value); // Add at new column 2 with same value

            // Проверьте изменение
            cell1 = scenario.InputCells[0];
            Console.WriteLine($"Modified first input cell column to: {cell1.Column}");

            // Сохраните книгу
            workbook.Save("ScenarioInputCellColumnDemo.xlsx");
        }
    }
}
```

### См. также

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


