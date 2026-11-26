---
title: "Класс Scenario"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Scenario класс. Представляет отдельный сценарий"
type: docs
url: /ru/net/aspose.cells/scenario/
---
## Scenario class

Представляет отдельный сценарий.

```csharp
public class Scenario
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Comment](../../aspose.cells/scenario/comment/) { get; set; } | Получает и задает комментарий сценария. |
| [InputCells](../../aspose.cells/scenario/inputcells/) { get; } | Получает входные ячейки сценария. |
| [IsHidden](../../aspose.cells/scenario/ishidden/) { get; set; } | Указывает, скрыт ли сценарий. |
| [IsLocked](../../aspose.cells/scenario/islocked/) { get; set; } | Указывает, заблокирован ли сценарий для редактирования, когда лист защищён. |
| [Name](../../aspose.cells/scenario/name/) { get; set; } | Получает и задает имя сценария. |
| [User](../../aspose.cells/scenario/user/) { get; } | Получает имя пользователя, последним изменившего сценарий. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ScenarioDemo
    {
        public static void ScenarioExample()
        {
            // Создать новую книгу и получить доступ к первому листу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить коллекцию сценариев листа
            ScenarioCollection scenarios = worksheet.Scenarios;

            // Добавить новый сценарий в коллекцию.
            int scenarioIndex = scenarios.Add("MyScenario");
            Scenario scenario = scenarios[scenarioIndex];

            // Установка свойств сценария
            scenario.Comment = "This is a test scenario.";
            scenario.Name = "TestScenario";
            scenario.IsHidden = false;
            scenario.IsLocked = true;

            // Доступ к свойствам только для чтения
            string user = scenario.User;
            ScenarioInputCellCollection inputCells = scenario.InputCells;

            // Сохраните книгу
            workbook.Save("ScenarioExample.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


