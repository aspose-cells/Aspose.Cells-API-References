---
title: "ScenarioInputCellCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ScenarioInputCellCollection. Obtient ScenarioInputCell par index dans la liste"
type: docs
url: /fr/net/aspose.cells/scenarioinputcellcollection/item/
---
## ScenarioInputCellCollection indexer

Obtient [`ScenarioInputCell`](../../scenarioinputcell/) par index dans la liste.

```csharp
public ScenarioInputCell this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'index spécifique dans la liste |

### Valeur de retour

L'objet [`ScenarioInputCell`](../../scenarioinputcell/)

### Exemples

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

            // Démontrer l'utilisation de la propriété Item
            ScenarioInputCell firstCell = inputCells[0];
            ScenarioInputCell secondCell = inputCells[1];

            Console.WriteLine($"First cell - Row: {firstCell.Row}, Column: {firstCell.Column}, Value: {firstCell.Value}");
            Console.WriteLine($"Second cell - Row: {secondCell.Row}, Column: {secondCell.Column}, Value: {secondCell.Value}");

            workbook.Save("ScenarioInputCellCollectionExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [ScenarioInputCell](../../scenarioinputcell/)
* class [ScenarioInputCellCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


