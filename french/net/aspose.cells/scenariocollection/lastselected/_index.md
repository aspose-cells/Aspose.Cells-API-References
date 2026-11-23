---
title: "ScenarioCollection.LastSelected"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ScenarioCollection. Indique quel scénario a été sélectionné en dernier par l'utilisateur pour être exécuté/affiché"
type: docs
url: /fr/net/aspose.cells/scenariocollection/lastselected/
---
## ScenarioCollection.LastSelected property

Indique quel scénario a été sélectionné en dernier par l'utilisateur pour être exécuté/affiché.

```csharp
public int LastSelected { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioCollectionPropertyLastSelectedDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des scénarios
            ScenarioCollection scenarios = worksheet.Scenarios;
            scenarios.Add("Scenario1");
            scenarios.Add("Scenario2");

            // Définissez le scénario actif et l'index sélectionné en dernier
            scenarios.ActiveIndex = 1;
            scenarios.LastSelected = 1;

            // Vérifiez et démontrez la propriété LastSelected
            Console.WriteLine("Total scenarios: " + scenarios.Count);
            Console.WriteLine("Active scenario index: " + scenarios.ActiveIndex);
            Console.WriteLine("Last selected scenario index: " + scenarios.LastSelected);

            // Modifiez l'index sélectionné en dernier
            scenarios.LastSelected = 0;
            Console.WriteLine("Updated last selected scenario index: " + scenarios.LastSelected);
        }
    }
}
```

### Voir aussi

* class [ScenarioCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


