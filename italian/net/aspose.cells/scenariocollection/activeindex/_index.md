---
title: "ScenarioCollection.ActiveIndex"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ScenarioCollection. Ottiene e imposta quale scenario è selezionato"
type: docs
url: /it/net/aspose.cells/scenariocollection/activeindex/
---
## ScenarioCollection.ActiveIndex property

Ottiene e imposta quale scenario è selezionato.

```csharp
public int ActiveIndex { get; set; }
```

### Esempi

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

### Vedi anche

* class [ScenarioCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


