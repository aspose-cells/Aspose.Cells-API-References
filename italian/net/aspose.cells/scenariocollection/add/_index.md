---
title: "ScenarioCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ScenarioCollection. Aggiunge uno scenario"
type: docs
url: /it/net/aspose.cells/scenariocollection/add/
---
## ScenarioCollection.Add method

Aggiunge uno scenario.

```csharp
public int Add(string name)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome dello scenario. |

### Valore di ritorno

L'indice nella lista degli scenari.

### Esempi

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

### Vedi anche

* class [ScenarioCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


