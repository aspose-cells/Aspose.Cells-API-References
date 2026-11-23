---
title: "Scenario.Comment"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Scenario. Obtient et définit le commentaire du scénario"
type: docs
url: /fr/net/aspose.cells/scenario/comment/
---
## Scenario.Comment property

Obtient et définit le commentaire du scénario.

```csharp
public string Comment { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioPropertyCommentDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une collection de scénarios
            ScenarioCollection scenarios = worksheet.Scenarios;
            
            // Ajouter un scénario
            int index = scenarios.Add("test");
            Scenario scenario = scenarios[index];
            
            // Définir les propriétés du scénario
            scenario.IsLocked = true;
            scenario.Comment = "创建者 Simon 日期 " + DateTime.Now.ToShortDateString();
            
            // Ajouter des cellules d'entrée au scénario en utilisant les références de cellules et les valeurs
            scenario.InputCells.Add(0, 6, "1");  // G16 (row 0, column 6)
            scenario.InputCells.Add(0, 0, "100"); // A1
            scenario.InputCells.Add(1, 1, "200"); // B2
            scenario.InputCells.Add(2, 2, "300"); // C3

            // Afficher le commentaire du scénario
            Console.WriteLine("Scenario Comment: " + scenario.Comment);
            
            // Enregistrez le classeur
            workbook.Save("ScenarioCommentDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Scenario](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


