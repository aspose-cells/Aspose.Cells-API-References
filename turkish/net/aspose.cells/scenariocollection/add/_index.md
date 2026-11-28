---
title: "ScenarioCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ScenarioCollection yöntemi. Bir senaryo ekler"
type: docs
url: /tr/net/aspose.cells/scenariocollection/add/
---
## ScenarioCollection.Add method

Bir senaryo ekler.

```csharp
public int Add(string name)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Senaryonun adı. |

### Dönüş Değeri

Senaryolar listesindeki indeks.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int scenarioIndex = worksheet.Scenarios.Add("Scenario1");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(0, 0, "100");
            inputCells.Add(1, 1, "200");

            Console.WriteLine("Scenario Name: " + scenario.Name);
            Console.WriteLine("Input Cell Count: " + inputCells.Count);
            Console.WriteLine($"First Cell - Row: {inputCells[0].Row}, Column: {inputCells[0].Column}, Value: {inputCells[0].Value}");

            workbook.Save("ScenarioCollectionAddDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ScenarioCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


