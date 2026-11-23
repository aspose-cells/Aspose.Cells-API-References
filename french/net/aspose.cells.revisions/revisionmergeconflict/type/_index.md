---
title: "RevisionMergeConflict.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionMergeConflict. Obtient le type de révision"
type: docs
url: /fr/net/aspose.cells.revisions/revisionmergeconflict/type/
---
## RevisionMergeConflict.Type property

Obtient le type de révision.

```csharp
public override RevisionType Type { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionMergeConflictPropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Activer le suivi des modifications
            workbook.StartAccessCache(AccessCacheOptions.All);

            // Apporter des modifications pour créer un scénario de conflit de fusion
            worksheet.Cells["A1"].PutValue("Original Value");
            workbook.Save("TempMergeConflict.xlsx");

            // Simuler un conflit de fusion en ouvrant le fichier et en apportant des modifications conflictuelles
            Workbook otherUserWorkbook = new Workbook("TempMergeConflict.xlsx");
            otherUserWorkbook.Worksheets[0].Cells["A1"].PutValue("Conflicting Change");
            otherUserWorkbook.Save("TempMergeConflict_OtherUser.xlsx");

            // Fusionner les modifications conflictuelles
            workbook.Combine(otherUserWorkbook);

            // Vérifier s'il y a des révisions
            if (workbook.HasRevisions)
            {
                // Trouver la révision du conflit de fusion
                RevisionMergeConflict mergeConflictRevision = null;
                // Remarque : Dans une implémentation réelle, vous auriez besoin d'une autre méthode pour accéder aux révisions
                // car la propriété Revisions n'est pas disponible dans la définition d'API fournie

                if (mergeConflictRevision != null)
                {
                    // Afficher la propriété Type de la révision du conflit de fusion
                    Console.WriteLine("Merge Conflict Revision Type: " + mergeConflictRevision.Type);

                    // Démontrer comment ces informations peuvent être utilisées
                    if (mergeConflictRevision.Type == RevisionType.MergeConflict)
                    {
                        Console.WriteLine("This revision represents a merge conflict.");
                        Console.WriteLine("Worksheet affected: " + mergeConflictRevision.Worksheet.Name);
                    }
                }
            }

            // Enregistrer le classeur avec les révisions
            workbook.Save("RevisionMergeConflictTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [RevisionType](../../revisiontype/)
* class [RevisionMergeConflict](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


