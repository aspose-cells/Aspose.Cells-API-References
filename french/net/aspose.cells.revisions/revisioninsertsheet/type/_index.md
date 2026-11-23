---
title: "RevisionInsertSheet.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionInsertSheet. Obtient le type de révision"
type: docs
url: /fr/net/aspose.cells.revisions/revisioninsertsheet/type/
---
## RevisionInsertSheet.Type property

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

    public class RevisionInsertSheetPropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur avec suivi des révisions
            Workbook workbook = new Workbook();
            
            // Activer le suivi des révisions (simulé car StartTrackingRevisions n'est pas disponible)
            bool trackRevisions = true;

            // Ajouter une nouvelle feuille de calcul pour générer un enregistrement de révision
            Worksheet newSheet = workbook.Worksheets.Add("NewSheet");
            
            // Simuler l'obtention des révisions (car la propriété Revisions n'est pas disponible)
            if (trackRevisions && workbook.HasRevisions)
            {
                // Dans un scénario réel, nous accéderions aux révisions ici
                // Cela suppose que nous avons obtenu la révision de quelque part (comme workbook.Revisions)
                RevisionInsertSheet insertSheetRevision = null; // Would be assigned from actual revisions collection
                
                if (insertSheetRevision != null)
                {
                    // Afficher la propriété Type
                    Console.WriteLine("Revision Type: " + insertSheetRevision.Type);

                    // Démontrer l'utilisation de la propriété Type en lecture seule
                    if (insertSheetRevision.Type == RevisionType.InsertSheet)
                    {
                        Console.WriteLine("This revision represents a sheet insertion operation");
                        
                        // Afficher des informations supplémentaires sur la feuille insérée
                        Console.WriteLine("Inserted sheet name: " + insertSheetRevision.Name);
                        Console.WriteLine("Sheet position: " + insertSheetRevision.SheetPosition);
                    }

                    // Vérifier par rapport aux autres types de révision
                    if (insertSheetRevision.Type != RevisionType.Unknown)
                    {
                        Console.WriteLine("This is a known revision type");
                    }
                }

                // Enregistrez le classeur
                workbook.Save("RevisionInsertSheetTypeDemo.xlsx");
            }
            else
            {
                Console.WriteLine("No revisions found or revision tracking not enabled");
            }
        }
    }
}
```

### Voir aussi

* enum [RevisionType](../../revisiontype/)
* class [RevisionInsertSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


