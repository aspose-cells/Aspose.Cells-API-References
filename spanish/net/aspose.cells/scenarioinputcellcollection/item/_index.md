---
title: "ScenarioInputCellCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "ScenarioInputCellCollection propiedad. Obtiene ScenarioInputCell por índice en la lista"
type: docs
url: /es/net/aspose.cells/scenarioinputcellcollection/item/
---
## ScenarioInputCellCollection indexer

Obtiene [`ScenarioInputCell`](../../scenarioinputcell/) por índice en la lista.

```csharp
public ScenarioInputCell this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice específico en la lista |

### Valor de retorno

El objeto [`ScenarioInputCell`](../../scenarioinputcell/)

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int scenarioIndex = worksheet.Scenarios.Add("Scenario1");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];
            ScenarioInputCellCollection inputCells = scenario.InputCells;

            inputCells.Add(0, 0, "10");
            inputCells.Add(1, 1, "20");

            // Demostrar el uso de la propiedad Item
            ScenarioInputCell firstCell = inputCells[0];
            ScenarioInputCell secondCell = inputCells[1];

            Console.WriteLine($"First cell - Row: {firstCell.Row}, Column: {firstCell.Column}, Value: {firstCell.Value}");
            Console.WriteLine($"Second cell - Row: {secondCell.Row}, Column: {secondCell.Column}, Value: {secondCell.Value}");

            workbook.Save("ScenarioInputCellCollectionExample.xlsx");
        }
    }
}
```

### Ver también

* class [ScenarioInputCell](../../scenarioinputcell/)
* class [ScenarioInputCellCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


