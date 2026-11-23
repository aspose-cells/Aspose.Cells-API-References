---
title: "Worksheet.TransitionEntry"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Indique si l'option de compatibilité Lotus Transition Formula Entry est activée"
type: docs
url: /fr/net/aspose.cells/worksheet/transitionentry/
---
## Worksheet.TransitionEntry property

Indique si l'option Transition Formula Entry (compatibilité Lotus) est activée.

```csharp
public bool TransitionEntry { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTransitionEntryDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir la propriété TransitionEntry
            worksheet.TransitionEntry = true;
            
            // Afficher la valeur de TransitionEntry
            Console.WriteLine("TransitionEntry: " + worksheet.TransitionEntry);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
            
            // Chargez le classeur enregistré pour vérifier la propriété
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // Afficher la valeur de TransitionEntry chargée
            Console.WriteLine("Loaded TransitionEntry: " + loadedWorksheet.TransitionEntry);
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


