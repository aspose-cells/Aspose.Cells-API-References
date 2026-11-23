---
title: "Revision.Worksheet"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Revision. Obtient la feuille de calcul"
type: docs
url: /fr/net/aspose.cells.revisions/revision/worksheet/
---
## Revision.Worksheet property

Obtient la feuille de calcul.

```csharp
public Worksheet Worksheet { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionPropertyWorksheetDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir les propriétés de la feuille de calcul
            worksheet.Name = "Demo Sheet";
            worksheet.IsGridlinesVisible = true;
            worksheet.DisplayZeros = false;
            worksheet.Zoom = 120;
            
            // Ajouter des données pour démontrer les révisions
            worksheet.Cells["A1"].PutValue("Original Value");
            
            // Protéger la feuille de calcul pour activer le suivi des modifications
            worksheet.Protect(ProtectionType.All);
            
            // Effectuer une modification qui sera suivie en tant que révision
            worksheet.Cells["A1"].PutValue("Modified Value");
            
            // Enregistrer le classeur pour suivre les révisions
            workbook.Save("RevisionDemo.xlsx");
            
            // Charger le classeur avec les révisions
            Workbook workbookWithRevisions = new Workbook("RevisionDemo.xlsx");
            
            // Accéder aux journaux de révision
            foreach (RevisionLog log in workbookWithRevisions.Worksheets.RevisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    // Démontrer l'accès à la propriété Worksheet depuis la révision
                    Console.WriteLine($"Revision Type: {revision.Type}");
                    Console.WriteLine($"Worksheet Name: {revision.Worksheet.Name}");
                    Console.WriteLine($"Worksheet Index: {revision.Worksheet.Index}");
                    
                    if (revision.Type == RevisionType.ChangeCells)
                    {
                        RevisionCellChange cellChange = (RevisionCellChange)revision;
                        Console.WriteLine($"Cell changed in worksheet '{cellChange.Worksheet.Name}': {cellChange.CellName}");
                    }
                }
            }
        }
    }
}
```

### Voir aussi

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [Revision](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


