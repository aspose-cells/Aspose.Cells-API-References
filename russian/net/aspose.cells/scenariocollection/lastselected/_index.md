---
title: "ScenarioCollection.LastSelected"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ScenarioCollection. Указывает, какой сценарий был выбран пользователем последним для выполнения/отображения"
type: docs
url: /ru/net/aspose.cells/scenariocollection/lastselected/
---
## ScenarioCollection.LastSelected property

Указывает, какой сценарий был последним выбран пользователем для выполнения/отображения.

```csharp
public int LastSelected { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioCollectionPropertyLastSelectedDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить сценарии
            ScenarioCollection scenarios = worksheet.Scenarios;
            scenarios.Add("Scenario1");
            scenarios.Add("Scenario2");

            // Установите активный сценарий и индекс последнего выбранного
            scenarios.ActiveIndex = 1;
            scenarios.LastSelected = 1;

            // Проверьте и продемонстрируйте свойство LastSelected
            Console.WriteLine("Total scenarios: " + scenarios.Count);
            Console.WriteLine("Active scenario index: " + scenarios.ActiveIndex);
            Console.WriteLine("Last selected scenario index: " + scenarios.LastSelected);

            // Измените индекс последнего выбранного
            scenarios.LastSelected = 0;
            Console.WriteLine("Updated last selected scenario index: " + scenarios.LastSelected);
        }
    }
}
```

### См. также

* class [ScenarioCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


