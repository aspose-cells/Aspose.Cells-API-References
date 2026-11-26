---
title: "ScenarioInputCell.Row"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ScenarioInputCell. Получает и задает индекс строки входной ячейки"
type: docs
url: /ru/net/aspose.cells/scenarioinputcell/row/
---
## ScenarioInputCell.Row property

Получает и задает индекс строки входной ячейки.

```csharp
public int Row { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyRowDemo
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

            // Получить доступ и продемонстрировать свойство Row
            ScenarioInputCell cell1 = scenario.InputCells[0];
            Console.WriteLine($"First input cell is at row: {cell1.Row}");

            // Добавьте новую ячейку во 2‑й строке вместо попытки изменить существующую
            worksheet.Cells[2, 0].Value = "30"; // Cell A3
            scenario.InputCells.Add(2, 0, "30");
            Console.WriteLine($"New input cell added at row: {scenario.InputCells[2].Row}");

            // Сохраните книгу
            workbook.Save("ScenarioInputCellRowDemo.xlsx");
        }
    }
}
```

### См. также

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


