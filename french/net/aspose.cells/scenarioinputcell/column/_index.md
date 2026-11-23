---
title: "ScenarioInputCell.Column"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ScenarioInputCell propriété. Obtient et définit l'index de colonne de la cellule d'entrée"
type: docs
url: /fr/net/aspose.cells/scenarioinputcell/column/
---
## ScenarioInputCell.Column property

Obtient et définit l'index de colonne de la cellule d'entrée.

```csharp
public int Column { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyColumnDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez un scénario à la feuille de calcul
            int scenarioIndex = worksheet.Scenarios.Add("Scenario1");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Ajoutez des cellules d'entrée au scénario
            scenario.InputCells.Add(0, 0, "10"); // Cell A1
            scenario.InputCells.Add(1, 1, "20"); // Cell B2

            // Accéder et démontrer la propriété Column
            ScenarioInputCell cell1 = scenario.InputCells[0];
            Console.WriteLine($"First input cell is at column: {cell1.Column}");

            // Comme Column est en lecture seule, nous devons la supprimer et la réajouter pour changer Column
            string value = cell1.Value;
            scenario.InputCells.RemoveAt(0);
            scenario.InputCells.Add(0, 2, value); // Add at new column 2 with same value

            // Vérifier le changement
            cell1 = scenario.InputCells[0];
            Console.WriteLine($"Modified first input cell column to: {cell1.Column}");

            // Enregistrez le classeur
            workbook.Save("ScenarioInputCellColumnDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


