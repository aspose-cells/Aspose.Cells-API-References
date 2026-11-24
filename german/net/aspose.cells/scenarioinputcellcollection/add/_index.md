---
title: "ScenarioInputCellCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ScenarioInputCellCollection-Methode. Fügt eine Eingabezelle hinzu"
type: docs
url: /de/net/aspose.cells/scenarioinputcellcollection/add/
---
## ScenarioInputCellCollection.Add method

Fügt eine Eingabezelle hinzu.

```csharp
public int Add(int row, int column, string value)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Der Zeilenindex der Eingabezelle. |
| column | Int32 | Der Spaltenindex der Eingabezelle. |
| Wert | String | Der Wert der Eingabezelle. |

### Beispiele

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

### Siehe auch

* class [ScenarioInputCellCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


