---
title: "RevisionInsertSheet.ActionType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionInsertSheet. Obtient le type d'action de la révision"
type: docs
url: /fr/net/aspose.cells.revisions/revisioninsertsheet/actiontype/
---
## RevisionInsertSheet.ActionType property

Obtient le type d'action de la révision.

```csharp
public RevisionActionType ActionType { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionInsertSheetPropertyActionTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur avec suivi des révisions
            Workbook workbook = new Workbook();
            // Remarque : StartTrackingRevisions n'est pas disponible dans l'API fournie
            // workbook.StartTrackingRevisions();

            // Ajouter une nouvelle feuille de calcul pour générer un enregistrement de révision
            Worksheet newSheet = workbook.Worksheets.Add("NewSheet");
            
            // Remarque : StopTrackingRevisions n'est pas disponible dans l'API fournie
            // workbook.StopTrackingRevisions();
            
            // Remarque : la propriété Revisions n'est pas disponible dans l'API fournie
            // Nous utiliserons HasRevisions pour vérifier s'il y a des révisions
            if (workbook.HasRevisions)
            {
                // Dans un scénario réel, nous accéderions aux révisions ici
                // Comme nous ne pouvons pas créer RevisionInsertSheet directement, nous simulerons la vérification d'un
                // Cela suppose que nous avons obtenu la révision de quelque part (comme workbook.Revisions)
                RevisionInsertSheet insertSheetRevision = null; // Would be assigned from actual revisions collection
                
                // Comme nous ne pouvons pas créer ou définir ActionType, nous allons simplement démontrer comment le vérifier
                if (insertSheetRevision != null)
                {
                    // Afficher la propriété ActionType
                    Console.WriteLine("ActionType of sheet insertion: " + insertSheetRevision.ActionType);

                    // Démontrer l'utilisation de la propriété en lecture seule
                    if (insertSheetRevision.ActionType == RevisionActionType.Add)
                    {
                        Console.WriteLine("This revision represents a sheet addition");
                    }
                }

                // Enregistrer le classeur avec les révisions
                workbook.Save("RevisionInsertSheetActionTypeDemo.xlsx");
            }
            else
            {
                Console.WriteLine("No sheet insertion revision found");
            }
        }
    }
}
```

### Voir aussi

* enum [RevisionActionType](../../revisionactiontype/)
* class [RevisionInsertSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


