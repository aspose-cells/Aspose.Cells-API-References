---
title: "ScenarioInputCell.IsDeleted"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ScenarioInputCell. Указывает, удалена ли входная ячейка"
type: docs
url: /ru/net/aspose.cells/scenarioinputcell/isdeleted/
---
## ScenarioInputCell.IsDeleted property

Указывает, удалена ли входная ячейка.

```csharp
public bool IsDeleted { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyIsDeletedDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить сценарий
            int scenarioIndex = worksheet.Scenarios.Add("TestScenario");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Добавить входные ячейки
            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(0, 0, "100");
            inputCells.Add(1, 1, "200");

            // Получить доступ и отобразить входные ячейки
            ScenarioInputCell cell1 = inputCells[0];
            Console.WriteLine($"Cell A1 - Value: {cell1.Value}, IsDeleted: {cell1.IsDeleted}");

            // Удалить первую входную ячейку
            cell1.IsDeleted = true;
            Console.WriteLine($"After deletion - Cell A1 IsDeleted: {cell1.IsDeleted}");

            // Сохраните книгу
            workbook.Save("ScenarioWithDeletedCell.xlsx");
        }
    }
}
```

### См. также

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


