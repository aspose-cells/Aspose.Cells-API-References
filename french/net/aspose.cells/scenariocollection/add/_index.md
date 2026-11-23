---
title: "ScenarioCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ScenarioCollection. Ajoute un scénario"
type: docs
url: /fr/net/aspose.cells/scenariocollection/add/
---
## ScenarioCollection.Add method

Ajoute un scénario.

```csharp
public int Add(string name)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom du scénario. |

### Valeur de retour

L'index dans la liste des scénarios.

### Exemples

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

### Voir aussi

* class [ScenarioCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


