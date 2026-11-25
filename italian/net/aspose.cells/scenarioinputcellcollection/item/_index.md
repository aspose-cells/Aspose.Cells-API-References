---
title: "ScenarioInputCellCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ScenarioInputCellCollection. Ottiene ScenarioInputCell per indice nell'elenco"
type: docs
url: /it/net/aspose.cells/scenarioinputcellcollection/item/
---
## ScenarioInputCellCollection indexer

Ottiene [`ScenarioInputCell`](../../scenarioinputcell/) per indice nell'elenco.

```csharp
public ScenarioInputCell this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice specifico nell'elenco |

### Valore di ritorno

L'oggetto [`ScenarioInputCell`](../../scenarioinputcell/)

### Esempi

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

            // Dimostra l'uso della proprietà Item
            ScenarioInputCell firstCell = inputCells[0];
            ScenarioInputCell secondCell = inputCells[1];

            Console.WriteLine($"First cell - Row: {firstCell.Row}, Column: {firstCell.Column}, Value: {firstCell.Value}");
            Console.WriteLine($"Second cell - Row: {secondCell.Row}, Column: {secondCell.Column}, Value: {secondCell.Value}");

            workbook.Save("ScenarioInputCellCollectionExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [ScenarioInputCell](../../scenarioinputcell/)
* class [ScenarioInputCellCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


