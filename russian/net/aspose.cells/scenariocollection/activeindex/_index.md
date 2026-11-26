---
title: "ScenarioCollection.ActiveIndex"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ScenarioCollection. Получает и задаёт, какой сценарий выбран"
type: docs
url: /ru/net/aspose.cells/scenariocollection/activeindex/
---
## ScenarioCollection.ActiveIndex property

Получает и задает, какой сценарий выбран.

```csharp
public int ActiveIndex { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioCollectionPropertyActiveIndexDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ScenarioCollection scenarios = worksheet.Scenarios;
            int scenarioIndex = scenarios.Add("TestScenario");
            
            scenarios.ActiveIndex = scenarioIndex;
            
            Console.WriteLine($"Active scenario index set to: {scenarios.ActiveIndex}");
            
            workbook.Save("ScenarioActiveIndexDemo.xlsx");
        }
    }
}
```

### См. также

* class [ScenarioCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


