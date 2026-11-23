---
title: "ScenarioInputCellCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ScenarioInputCellCollection. Ajoute une cellule d'entrée"
type: docs
url: /fr/net/aspose.cells/scenarioinputcellcollection/add/
---
## ScenarioInputCellCollection.Add method

Ajoute une cellule d'entrée.

```csharp
public int Add(int row, int column, string value)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | L'index de ligne de la cellule d'entrée. |
| column | Int32 | L'index de colonne de la cellule d'entrée. |
| valeur | String | La valeur de la cellule d'entrée. |

### Exemples

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

### Voir aussi

* class [ScenarioInputCellCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


