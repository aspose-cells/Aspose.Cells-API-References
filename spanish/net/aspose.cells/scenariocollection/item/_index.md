---
title: "ScenarioCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ScenarioCollection. Obtiene el objeto Scenario por el índice"
type: docs
url: /es/net/aspose.cells/scenariocollection/item/
---
## ScenarioCollection indexer

Obtiene el objeto [`Scenario`](../../scenario/) por el índice.

```csharp
public Scenario this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice específico en la lista. |

### Ejemplos

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

            // Demostrar el uso de la propiedad Item
            ScenarioInputCell firstCell = scenario.InputCells[0];
            Console.WriteLine($"First cell - Row: {firstCell.Row}, Column: {firstCell.Column}, Value: {firstCell.Value}");

            workbook.Save("ScenarioCollectionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Scenario](../../scenario/)
* class [ScenarioCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


