---
title: "Scenario.InputCells"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Scenario. Obtient les cellules d'entrée du scénario"
type: docs
url: /fr/net/aspose.cells/scenario/inputcells/
---
## Scenario.InputCells property

Obtient les cellules d'entrée du scénario.

```csharp
public ScenarioInputCellCollection InputCells { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioPropertyInputCellsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez un scénario à la feuille de calcul
            int scenarioIndex = worksheet.Scenarios.Add("Scenario 1");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Ajouter des cellules d'entrée au scénario en utilisant la propriété InputCells
            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(0, 0, "100"); // Cell A1
            inputCells.Add(1, 1, "200"); // Cell B2

            // Modifier la valeur de la première cellule d'entrée
            inputCells[0].Value = "150";

            // Enregistrez le classeur
            workbook.Save("ScenarioInputCellsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ScenarioInputCellCollection](../../scenarioinputcellcollection/)
* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


