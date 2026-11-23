---
title: "ScenarioInputCell.Row"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ScenarioInputCell propriété. Obtient et définit l'index de ligne de la cellule d'entrée"
type: docs
url: /fr/net/aspose.cells/scenarioinputcell/row/
---
## ScenarioInputCell.Row property

Obtient et définit l'index de ligne de la cellule d'entrée.

```csharp
public int Row { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioInputCellPropertyRowDemo
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

            // Accéder et démontrer la propriété Row
            ScenarioInputCell cell1 = scenario.InputCells[0];
            Console.WriteLine($"First input cell is at row: {cell1.Row}");

            // Ajouter une nouvelle cellule à la ligne 2 au lieu d'essayer de modifier celle existante
            worksheet.Cells[2, 0].Value = "30"; // Cell A3
            scenario.InputCells.Add(2, 0, "30");
            Console.WriteLine($"New input cell added at row: {scenario.InputCells[2].Row}");

            // Enregistrez le classeur
            workbook.Save("ScenarioInputCellRowDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ScenarioInputCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


