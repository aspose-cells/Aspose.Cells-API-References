---
title: "ScenarioCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ScenarioCollection özelliği. İndekse göre Scenario nesnesini alır"
type: docs
url: /tr/net/aspose.cells/scenariocollection/item/
---
## ScenarioCollection indexer

İndekse göre [`Scenario`](../../scenario/) nesnesini alır.

```csharp
public Scenario this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | Listede belirli indeks. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int scenarioIndex = worksheet.Scenarios.Add("TestScenario");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            scenario.InputCells.Add(0, 0, "100");
            scenario.InputCells.Add(1, 1, "200");

            // Item özelliğinin kullanımını göster
            ScenarioInputCell firstCell = scenario.InputCells[0];
            Console.WriteLine($"First cell - Row: {firstCell.Row}, Column: {firstCell.Column}, Value: {firstCell.Value}");

            workbook.Save("ScenarioCollectionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Scenario](../../scenario/)
* class [ScenarioCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


