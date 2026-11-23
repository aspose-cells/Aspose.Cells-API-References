---
title: "ScenarioInputCell.Value"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ScenarioInputCell propriété. Obtient et définit la valeur de la cellule d'entrée"
type: docs
url: /fr/net/aspose.cells/scenarioinputcell/value/
---
## ScenarioInputCell.Value property

Obtient et définit la valeur de la cellule d'entrée.

```csharp
public string Value { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyValueDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un scénario
            int scenarioIndex = worksheet.Scenarios.Add("TestScenario");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Ajouter des cellules d'entrée avec des valeurs
            scenario.InputCells.Add(0, 0, "100"); // Cell A1
            scenario.InputCells.Add(1, 1, "200"); // Cell B2

            // Accéder et modifier les valeurs
            ScenarioInputCell cell1 = scenario.InputCells[0];
            Console.WriteLine($"Original value: {cell1.Value}");
            cell1.Value = "150"; // Modify the value
            Console.WriteLine($"Modified value: {cell1.Value}");

            // Enregistrez le classeur
            workbook.Save("ScenarioValueDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


