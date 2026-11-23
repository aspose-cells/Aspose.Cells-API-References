---
title: "ScenarioInputCell.IsDeleted"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ScenarioInputCell propriété. Indique si la cellule d'entrée est supprimée"
type: docs
url: /fr/net/aspose.cells/scenarioinputcell/isdeleted/
---
## ScenarioInputCell.IsDeleted property

Indique si la cellule d'entrée est supprimée.

```csharp
public bool IsDeleted { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyIsDeletedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un scénario
            int scenarioIndex = worksheet.Scenarios.Add("TestScenario");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Ajouter des cellules d'entrée
            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(0, 0, "100");
            inputCells.Add(1, 1, "200");

            // Accéder et afficher les cellules d'entrée
            ScenarioInputCell cell1 = inputCells[0];
            Console.WriteLine($"Cell A1 - Value: {cell1.Value}, IsDeleted: {cell1.IsDeleted}");

            // Supprimer la première cellule d'entrée
            cell1.IsDeleted = true;
            Console.WriteLine($"After deletion - Cell A1 IsDeleted: {cell1.IsDeleted}");

            // Enregistrez le classeur
            workbook.Save("ScenarioWithDeletedCell.xlsx");
        }
    }
}
```

### Voir aussi

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


