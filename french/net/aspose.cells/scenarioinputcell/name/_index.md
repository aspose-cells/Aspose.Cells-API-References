---
title: "ScenarioInputCell.Name"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ScenarioInputCell propriété. Obtient et définit l'adresse de la cellule d'entrée"
type: docs
url: /fr/net/aspose.cells/scenarioinputcell/name/
---
## ScenarioInputCell.Name property

Obtient et définit l'adresse de la cellule d'entrée.

```csharp
public string Name { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer un scénario
            ScenarioCollection scenarios = worksheet.Scenarios;
            int scenarioIndex = scenarios.Add("TestScenario");

            // Obtenir le scénario
            Scenario scenario = scenarios[scenarioIndex];

            // Ajoutez des cellules d'entrée au scénario
            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(6, 15, "1"); // G16 is row 6, column 15 (0-based)
            inputCells.Add(7, 15, "2"); // H16 is row 7, column 15 (0-based)

            // Obtenir les cellules d'entrée
            ScenarioInputCell inputCell1 = inputCells[0];
            ScenarioInputCell inputCell2 = inputCells[1];

            // Démontrer l'utilisation de la propriété Name
            Console.WriteLine("First input cell name: " + inputCell1.Name);
            Console.WriteLine("Second input cell name: " + inputCell2.Name);

            // Vérifier que les noms correspondent aux valeurs attendues
            if (inputCell1.Name != "G16" || inputCell2.Name != "H16")
            {
                throw new Exception("Input cell names don't match expected values");
            }
        }
    }
}
```

### Voir aussi

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


