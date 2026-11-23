---
title: "Classe Scenario"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Scenario. Représente un scénario individuel"
type: docs
url: /fr/net/aspose.cells/scenario/
---
## Scenario class

Représente un scénario individuel.

```csharp
public class Scenario
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Comment](../../aspose.cells/scenario/comment/) { get; set; } | Obtient et définit le commentaire du scénario. |
| [InputCells](../../aspose.cells/scenario/inputcells/) { get; } | Obtient les cellules d'entrée du scénario. |
| [IsHidden](../../aspose.cells/scenario/ishidden/) { get; set; } | Indique si le scénario est masqué. |
| [IsLocked](../../aspose.cells/scenario/islocked/) { get; set; } | Indique si le scénario est verrouillé pour l'édition lorsque la feuille est protégée. |
| [Name](../../aspose.cells/scenario/name/) { get; set; } | Obtient et définit le nom du scénario. |
| [User](../../aspose.cells/scenario/user/) { get; } | Obtient le nom de l'utilisateur qui a modifié le scénario en dernier. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ScenarioDemo
    {
        public static void ScenarioExample()
        {
            // Créer un nouveau classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder à la collection de scénarios de la feuille de calcul
            ScenarioCollection scenarios = worksheet.Scenarios;

            // Ajoutez un nouveau scénario à la collection
            int scenarioIndex = scenarios.Add("MyScenario");
            Scenario scenario = scenarios[scenarioIndex];

            // Définir les propriétés du scénario
            scenario.Comment = "This is a test scenario.";
            scenario.Name = "TestScenario";
            scenario.IsHidden = false;
            scenario.IsLocked = true;

            // Accéder aux propriétés en lecture seule
            string user = scenario.User;
            ScenarioInputCellCollection inputCells = scenario.InputCells;

            // Enregistrez le classeur
            workbook.Save("ScenarioExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


