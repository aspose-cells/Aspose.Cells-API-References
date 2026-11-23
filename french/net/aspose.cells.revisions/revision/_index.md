---
title: "Classe Revision"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Revisions.Revision class. Représente la révision"
type: docs
url: /fr/net/aspose.cells.revisions/revision/
---
## Revision class

Représente la révision.

```csharp
public abstract class Revision
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Obtient le numéro de cette révision. |
| virtual [Type](../../aspose.cells.revisions/revision/type/) { get; } | Représente le type de révision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Obtient la feuille de calcul. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Ajouter des données susceptibles de créer des révisions
                worksheet.Cells["A1"].PutValue("Original Value");

                // Enregistrer le classeur pour établir une base de référence
                workbook.Save("RevisionDemo_Baseline.xlsx");

                // Charger le classeur et effectuer une modification
                Workbook modifiedWorkbook = new Workbook("RevisionDemo_Baseline.xlsx");
                modifiedWorkbook.Worksheets[0].Cells["A1"].PutValue("Modified Value");

                // Vérifier s'il existe des journaux de révision
                if (modifiedWorkbook.Worksheets.RevisionLogs.Count > 0)
                {
                    RevisionLog log = modifiedWorkbook.Worksheets.RevisionLogs[0];
                    if (log.Revisions.Count > 0)
                    {
                        // Obtenir la première révision
                        Revision revision = log.Revisions[0];

                        // Afficher les propriétés en lecture seule
                        Console.WriteLine($"Revision ID: {revision.Id}");
                        Console.WriteLine($"Revision Type: {revision.Type}");
                        Console.WriteLine($"Worksheet Name: {revision.Worksheet.Name}");

                        // Enregistrer le classeur modifié
                        modifiedWorkbook.Save("RevisionDemo_Modified.xlsx");
                    }
                    else
                    {
                        Console.WriteLine("No revisions found in the log");
                    }
                }
                else
                {
                    Console.WriteLine("No revision logs available");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with Revision: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


