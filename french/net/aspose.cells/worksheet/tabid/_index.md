---
title: "Worksheet.TabId"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Spécifie l'identifiant interne de la feuille"
type: docs
url: /fr/net/aspose.cells/worksheet/tabid/
---
## Worksheet.TabId property

Spécifie l'identifiant interne de la feuille.

```csharp
public int TabId { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTabIdDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir la propriété TabId
            worksheet.TabId = 107;
            
            // Enregistrez le classeur
            string outputPath = "output.xlsb";
            workbook.Save(outputPath);
            
            // Charger le classeur enregistré pour vérifier le TabId
            Workbook loadedWorkbook = new Workbook(outputPath);
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // Afficher la valeur du TabId
            Console.WriteLine("Worksheet TabId: " + loadedWorksheet.TabId);
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


