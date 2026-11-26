---
title: "ScenarioCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ScenarioCollection. Añade un escenario"
type: docs
url: /es/net/aspose.cells/scenariocollection/add/
---
## ScenarioCollection.Add method

Agrega un escenario.

```csharp
public int Add(string name)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre del escenario. |

### Valor de retorno

El índice en la lista de escenarios.

### Ejemplos

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

### Ver también

* class [ScenarioCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


