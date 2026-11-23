---
title: "Worksheet.TransitionEvaluation"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Indique si l'option de compatibilité Lotus d'évaluation de formule de transition est activée"
type: docs
url: /fr/net/aspose.cells/worksheet/transitionevaluation/
---
## Worksheet.TransitionEvaluation property

Indique si l'option Transition Formula Evaluation (compatibilité Lotus) est activée.

```csharp
public bool TransitionEvaluation { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTransitionEvaluationDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir la propriété TransitionEvaluation
            worksheet.TransitionEvaluation = true;
            
            // Afficher la valeur de la propriété
            Console.WriteLine("TransitionEvaluation: " + worksheet.TransitionEvaluation);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
            
            // Chargez le classeur enregistré pour vérifier la propriété
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            Console.WriteLine("Loaded TransitionEvaluation: " + loadedWorksheet.TransitionEvaluation);
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


