---
title: "ScenarioInputCellCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ScenarioInputCellCollection-Eigenschaft. Gibt ScenarioInputCell anhand des Index in der Liste zurück"
type: docs
url: /de/net/aspose.cells/scenarioinputcellcollection/item/
---
## ScenarioInputCellCollection indexer

Gibt [`ScenarioInputCell`](../../scenarioinputcell/) anhand des Index in der Liste zurück.

```csharp
public ScenarioInputCell this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der spezifische Index in der Liste |

### Rückgabewert

Das [`ScenarioInputCell`](../../scenarioinputcell/)‑Objekt

### Beispiele

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

            // Demonstriere die Verwendung der Item-Eigenschaft
            ScenarioInputCell firstCell = inputCells[0];
            ScenarioInputCell secondCell = inputCells[1];

            Console.WriteLine($"First cell - Row: {firstCell.Row}, Column: {firstCell.Column}, Value: {firstCell.Value}");
            Console.WriteLine($"Second cell - Row: {secondCell.Row}, Column: {secondCell.Column}, Value: {secondCell.Value}");

            workbook.Save("ScenarioInputCellCollectionExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [ScenarioInputCell](../../scenarioinputcell/)
* class [ScenarioInputCellCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


