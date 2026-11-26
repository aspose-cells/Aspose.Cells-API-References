---
title: "Scenario.Comment"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Scenario. Получает и задаёт комментарий сценария"
type: docs
url: /ru/net/aspose.cells/scenario/comment/
---
## Scenario.Comment property

Получает и задает комментарий сценария.

```csharp
public string Comment { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioPropertyCommentDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать коллекцию сценариев
            ScenarioCollection scenarios = worksheet.Scenarios;
            
            // Добавить сценарий
            int index = scenarios.Add("test");
            Scenario scenario = scenarios[index];
            
            // Установить свойства сценария
            scenario.IsLocked = true;
            scenario.Comment = "创建者 Simon 日期 " + DateTime.Now.ToShortDateString();
            
            // Добавьте входные ячейки в сценарий, используя ссылки на ячейки и значения
            scenario.InputCells.Add(0, 6, "1");  // G16 (row 0, column 6)
            scenario.InputCells.Add(0, 0, "100"); // A1
            scenario.InputCells.Add(1, 1, "200"); // B2
            scenario.InputCells.Add(2, 2, "300"); // C3

            // Отобразить комментарий сценария
            Console.WriteLine("Scenario Comment: " + scenario.Comment);
            
            // Сохраните книгу
            workbook.Save("ScenarioCommentDemo.xlsx");
        }
    }
}
```

### См. также

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


