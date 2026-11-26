---
title: "ScenarioInputCellCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "ScenarioInputCellCollection método. Añade una celda de entrada"
type: docs
url: /es/net/aspose.cells/scenarioinputcellcollection/add/
---
## ScenarioInputCellCollection.Add method

Agrega una celda de entrada.

```csharp
public int Add(int row, int column, string value)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | El índice de fila de la celda de entrada. |
| columna | Int32 | El índice de columna de la celda de entrada. |
| valor | String | El valor de la celda de entrada. |

### Ejemplos

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

### Ver también

* class [ScenarioInputCellCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


