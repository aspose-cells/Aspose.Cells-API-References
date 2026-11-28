---
title: "ScenarioInputCellCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ScenarioInputCellCollection yöntemi. Bir giriş hücresi ekler"
type: docs
url: /tr/net/aspose.cells/scenarioinputcellcollection/add/
---
## ScenarioInputCellCollection.Add method

Bir giriş hücresi ekler.

```csharp
public int Add(int row, int column, string value)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Giriş hücresinin satır indeksi. |
| sütun | Int32 | Giriş hücresinin sütun indeksi. |
| değer | String | Giriş hücresinin değeri. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellCollectionMethodAddWithInt32Int32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int scenarioIndex = worksheet.Scenarios.Add("TestScenario");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];
            ScenarioInputCellCollection inputCells = scenario.InputCells;

            inputCells.Add(0, 0, "10");
            inputCells.Add(1, 1, "20");

            Console.WriteLine($"Count: {inputCells.Count}");
            Console.WriteLine($"Cell 1: Row={inputCells[0].Row}, Column={inputCells[0].Column}, Value={inputCells[0].Value}");
            Console.WriteLine($"Cell 2: Row={inputCells[1].Row}, Column={inputCells[1].Column}, Value={inputCells[1].Value}");

            workbook.Save("ScenarioInputCellCollectionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ScenarioInputCellCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


