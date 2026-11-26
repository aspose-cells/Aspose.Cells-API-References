---
title: "Scenario.InputCells"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Scenario. Возвращает входные ячейки сценария"
type: docs
url: /ru/net/aspose.cells/scenario/inputcells/
---
## Scenario.InputCells property

Получает входные ячейки сценария.

```csharp
public ScenarioInputCellCollection InputCells { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioPropertyInputCellsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить сценарий в рабочий лист
            int scenarioIndex = worksheet.Scenarios.Add("Scenario 1");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Добавить входные ячейки в сценарий, используя свойство InputCells
            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(0, 0, "100"); // Cell A1
            inputCells.Add(1, 1, "200"); // Cell B2

            // Изменить значение первой входной ячейки
            inputCells[0].Value = "150";

            // Сохраните книгу
            workbook.Save("ScenarioInputCellsDemo.xlsx");
        }
    }
}
```

### См. также

* class [ScenarioInputCellCollection](../../scenarioinputcellcollection/)
* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


