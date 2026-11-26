---
title: "Worksheet.Scenarios"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Возвращает коллекцию Scenario"
type: docs
url: /ru/net/aspose.cells/worksheet/scenarios/
---
## Worksheet.Scenarios property

Возвращает коллекцию [`Scenario`](../../scenario/).

```csharp
public ScenarioCollection Scenarios { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyScenariosDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте некоторые данные в ячейки
            worksheet.Cells["A1"].PutValue("Initial Value");
            worksheet.Cells["A2"].PutValue(100);
            
            // Добавить сценарии
            ScenarioCollection scenarios = worksheet.Scenarios;
            int scenarioIndex1 = scenarios.Add("Scenario1");
            Scenario scenario1 = scenarios[scenarioIndex1];
            scenario1.Comment = "First test scenario";
            
            int scenarioIndex2 = scenarios.Add("Scenario2");
            Scenario scenario2 = scenarios[scenarioIndex2];
            scenario2.Comment = "Second test scenario";
            
            // Сохраните книгу
            workbook.Save("WorksheetPropertyScenariosDemo.xlsx");
            
            // Очистить сценарии и сохранить снова
            scenarios.Clear();
            workbook.Save("WorksheetPropertyScenariosDemo_Cleared.xlsx");
        }
    }
}
```

### См. также

* class [ScenarioCollection](../../scenariocollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


